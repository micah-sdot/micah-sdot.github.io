---
layout: project
type: project
image: img/CatchTurtle/images.jpg
title: "Catch a Turtle"
date: 2023
published: false
labels:
  - Application
  - Meteor
  - Javascript
summary: "A project done for the Hawaii Annual Code Challenge"
---


<div class="text-center p-4">
  <img width="300px" src="../img/CatchTurtle/Screenshot 2023-08-31 171631.png" class="img-thumbnail" >
  <img width="300px" src="../img/CatchTurtle/Screenshot 2023-08-31 171650.png" class="img-thumbnail" >
  <img width="300px" src="../img/CatchTurtle/Screenshot 2023-08-31 171707.png" class="img-thumbnail" >
</div>

## What was it?

This was a project for the Hawaii Annual Code Challenge in 2023. It is an application that wanted the ability to keep track of reusable containers for food vendors at events. The general idea behind our website is that the vendors can keep track of how many containers they all have, so it has an inventory system. When a customer makes an order, the vendor uses the checkout tab to take containers away from the database and add the order to the order page. After each order is added, a QR code is shown for the customer that leads to a payment page for them to pay. The program also gives the customer a random ID number as an identifier to connect the person to the order when they return their container/containers so they can get their compensation when they return it. 

## My Role

I had two main parts, the order page and the add container page. Since these pages were my responsibility, it also meant that I had to create the Mongo databases for the containers and the customers. I will first start with the add page since that is what I finished first.

### Add Container

The Add page is actually very simple. First, I had to create a database that consisted of containers. That was pretty easy to begin with as all there was to do was to be able to add containers with the attributes of the size of the container, and the vendor who owns the container. The add page just basically adds the amount of containers the user wants to add to their inventory so they can keep track of it in their database. 

### List Orders

The list order page was not that hard as well except for one part. I first created a database for customers that included the customer's name, the order ID, and the container and the amount. Then, I put every single order inside of a table on the list order page since it makes it easier for the vendor to be able to see all of their orders. But there are certain instances where the vendor may have hundreds of orders at a time, and it would not be good for the user if they had to scroll through hundreds of orders trying to find one. So I added a search bar for the table that would filter the table in real time based on the letters you type and if it matches the name connected to the order. This one was a little tough for me at first. I put an input box at the top of the table for the user to input the names. Then I used a regex and use state to update the table to match the letters the user typed in and show multiple different names of different orders. 

## Problems and Fixes
It definitely is not the nicest-looking game in the world, but given what we had to use, I would say that it turned out pretty well. 
