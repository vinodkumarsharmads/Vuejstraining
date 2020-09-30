<template>
  <div id="app">
    <div class="header">
      <div class="t_header">
        <div class="container">
          <div class="logo">
            <a href="index.html">
              <img src="img/logo.png" alt />
            </a>
          </div>
          <ul class="header-social-icon">
            <li>
              <a href="#">
                <i class="fa fa-facebook" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-twitter" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-google-plus" aria-hidden="true"></i>
              </a>
            </li>
            <li>
              <a href="#">
                <i class="fa fa-rss" aria-hidden="true"></i>
              </a>
            </li>
          </ul>
        </div>
      </div>
      <div class="t_nav" id="navbar-main">
        <div class="container relative">
          <nav class="navbar navbar-inverse">
            <div class="container-fluid">
              <div class="navbar-header">
                <button
                  type="button"
                  class="navbar-toggle"
                  data-toggle="collapse"
                  data-target="#myNavbar"
                >
                  <span class="icon-bar"></span>
                  <span class="icon-bar"></span>
                  <span class="icon-bar"></span>
                </button>
              </div>
              <div class="collapse navbar-collapse" id="myNavbar">
                <ul class="top_nav" id="nav">
                  <li>
                    <router-link to="/">Home</router-link>
                  </li>
                  <li>
                    <router-link to="/contact">Contact Us</router-link>
                  </li>
                </ul>
              </div>
            </div>
          </nav>
        </div>
      </div>
    </div>
    <div class="clr"></div>
    <div class="container">
      <router-view />
    </div>
  </div>
</template>
  <style scoped>
  @import "//fonts.googleapis.com/css?family=Lato:300,400,700,900";
  @import "../public/css/bootstrap.css";
  @import "../public/css/easy-responsive-tabs.css";
  @import "../public/css/font-awesome.css";
  @import "../public/css/component.css";
  @import "../public/css/main.css";
  @import "../public/css/reponsive.css";
  @import "../public/css/animate.css";
  </style>
<style lang="stylus"></style>