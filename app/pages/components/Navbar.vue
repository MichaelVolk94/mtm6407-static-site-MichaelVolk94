<template>
    <nav>
      <ul>
        <li><a href="/">Home</a></li>
        <li><a href="/about">About</a></li>
        <li><a href="/photos">Photos</a></li>
        <li><a href="/contact">Contact</a></li>
      </ul>
    </nav>
  </template>
  
  <style>
  nav ul {
    display: flex;
    gap: 1rem;
    list-style: none;
  }
  nav ul li a {
    text-decoration: none;
    color: rgb(0, 102, 255);
  }
  </style>