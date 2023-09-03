<script>
export default {
  data() {
    return {
      currentYear: new Date().getFullYear(),
    };
  },
};
</script>

<template>
    <div class="footer">
      <div class="footerPadding">
        <!-- Top section -->
        <div class="footerTop">
          <!-- Logo -->
          <h2 class="footerLogo">Site</h2>
          <!-- Links -->
          <div class="footerLinks">
            <!-- Contact info -->
            <div class="footerLinksDiv">
              <h4>Get in touch</h4>
              <p>contact@site.com</p>
            </div>
            <!-- Social media links -->
            <div class="footerLinksDiv">
              <h4>Connect</h4>
              <div class="socialmedia">
                <a href="https://www.linkedin.com">
                  <span class="icon">🔗</span>
                  LinkedIn
                </a>
                <a href="https://github.com/">
                  <span class="icon">🐱</span>
                  GitHub
                </a>
              </div>
            </div>
          </div>
        </div>
        <!-- Bottom section -->
        <hr />
        <div class="footerBelow">
          <div class="footerCopyright">
            <p>@{{ currentYear }} Site - All rights reserved</p>
          </div>
        </div>
      </div>
    </div>
  </template>
  

<style>
.footer {
  background-color: #2d2d2d;
  color: white;
  position: absolute;
  bottom: 0;
  width: 100%;
}

.footerPadding {
  padding: 1rem;
  display: flex;
  flex-direction: column;
}

.footerLinks {
  display: flex;
  justify-content: space-around;
  align-items: flex-start;
  flex-wrap: wrap;
  width: 100%;
  text-align: left;
  margin-bottom: 2rem;
}

.footerLinksDiv {
  display: flex;
  align-items: flex-start;
  flex-direction: column;
  flex-wrap: wrap;
  width: 150px;
  text-align: left;
}

a {
  text-decoration: none;
  color: white;
  padding: 10px;
}

.socialmedia a {
  display: flex;
  align-items: center;
  margin-bottom: 10px;
}

.socialmedia span {
  margin-left: 10px;
}

.socialmedia .icon {
  margin-right: 10px;
}

.footerBelow {
  display: flex;
  justify-content: center;
  align-items: center;
  margin-bottom: 5px;
  margin-top: 2rem;
}

hr {
  color: white;
  width: 90%;
  margin-top: 1rem;
}

.footerBelow p {
  font-size: 13px;
  line-height: 15px;
  color: white;
  font-weight: 600;
  padding-bottom: 5px;
}

.footerTop {
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-bottom: 5px;
}

.footerLogo {
  margin-bottom: 1rem;
  font-size: 24px;
  font-weight: bold;
}
</style>