---
permalink: /contact/
title: "Contact Me"
author_profile: true
comments: false
---

<form 
  action="https://formspree.io/f/mgvebllw" 
  method="POST" 
  style="
    width: 100%; 
    margin: 20px auto; 
    padding: 20px; 
    border-radius: 15px; 
    background-color: #fff; 
    box-shadow: 0 4px 10px rgba(0, 0, 0, 0.1); 
    font-family: Arial, sans-serif; 
    color: #333;"
>
  <input 
    type="email" 
    name="email" 
    placeholder="Your Email" 
    required 
    style="
      width: 100%; 
      padding: 10px; 
      margin-bottom: 15px; 
      border: 1px solid #ccc; 
      border-radius: 10px; 
      background-color: #f9f9f9; 
      color: #333; 
      box-sizing: border-box;"
  >
  <input 
    type="text" 
    name="name" 
    placeholder="Your Name" 
    required 
    style="
      width: 100%; 
      padding: 10px; 
      margin-bottom: 15px; 
      border: 1px solid #ccc; 
      border-radius: 10px; 
      background-color: #f9f9f9; 
      color: #333; 
      box-sizing: border-box;"
  >
  <textarea 
    name="message" 
    placeholder="Your Message" 
    required 
    style="
      width: 100%; 
      height: 100px; 
      padding: 10px; 
      margin-bottom: 15px; 
      border: 1px solid #ccc; 
      border-radius: 10px; 
      background-color: #f9f9f9; 
      color: #333; 
      box-sizing: border-box;"
  ></textarea>
  <div style="display: flex; justify-content: center;">
    <button 
      type="submit" 
      style="
        width: 20%; 
        padding: 10px; 
        background-color: #52adc8; 
        color: white; 
        border: none; 
        border-radius: 20px; 
        cursor: pointer; 
        font-size: 16px; 
        box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);"
    >
      Send
    </button>
  </div>
</form>

<style>
  button:hover {
    transform: scale(1.075); 
    transition: all 0.3s ease; 
  }
</style>