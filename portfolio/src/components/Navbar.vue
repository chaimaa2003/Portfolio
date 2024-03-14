<template>
 
    <div class="nav" >
        <div class="img">
            <img
                src="@/assets/logo.png"
                alt=""
            />
        </div>
  
        <ul >
            <li>
                <a href="#">Home</a>
            </li>
            <li>
                <a href="#">Courses</a>
            </li>
            <li><a href="#">Careers</a></li>
            <li>
                <a href="#">Blog</a>
            </li>
            <li><a href="#">About Us</a></li>
        </ul>
    </div>
   
  </template>
  
  <script>
  export default {
    name: 'navbar',
  
    data() {
        return {
            isopen: false,
            isopen1: false,
        };
    },
  
    methods: {
        toggleLogin() {
            this.isopen = !this.isopen;
        },
        toggleSignup() {
            this.isopen1 = !this.isopen1;
        },
    },
  };
  </script>
  
  <style scoped>
  button {
    border: 0ch;
  }
  
  .img {
    width: 70px;
    height: 49px;
   
  }
  img {
    width: 100%;
    height: 100%;
    margin-top: -31px;
   
  }
  .nav {
    width: 100%;
    height: 80px;
    background-color: #fdfdfd;
    display: flex;
    align-items: center;
    padding-left: 20px;
    
  
  
  }
  ul {
    position: absolute;
    left: 300px;
    top: 25px;
    margin: 0px;
    padding: 0;
    list-style: none;
    display: inline;
    text-align: center;
  }
  li {
    display: table-cell;
    position: relative;
    font-family: Poppins;
    font-size: 16px;
    font-style: normal;
    font-weight: 300;
    line-height: normal;
    letter-spacing: 0.44px;
  }
  a {
    color: #000000;
    text-decoration: none;
    letter-spacing: 0.15em;
  
    display: inline-block;
    padding-left: 20px;
    padding-right: 20px;
    padding-bottom: 5px;
  
    position: inline;
  }
  a:after {
    background: none repeat scroll 0 0 transparent;
    bottom: -10%;
    content: '';
    display: block;
    height: 2px;
    left: 50%;
    position: absolute;
    background: #070707;
    transition: width 0.3s ease 0s, left 0.3s ease 0s;
    width: 0;
  }
  a:hover:after {
    width: 100%;
    left: 0;
    color: rgb(6, 16, 16);
  }
  </style>
  