---
layout: post
title:      "Authenticate: The Bouncer"
date:       2020-07-14 02:24:34 +0000
permalink:  authenticate_the_bouncer
---


Authentication in coding essentially serves as a safety net for program or user generated content in the database to ensure that the person attempting to access it is a person who ought to be accessing it. When the user attempts to access a specific piece or group of content, they are sending a request to the app server saying "Hey, I'd like to create/ update/ destroy, may I please?" The authentication is a figurative barrier between the user and that content that the server has to decide whether they are allowed to interact with and in what ways. The request is generally sent in the form of an HTTP header for the program to read, and if, for instance, the user sends a request that doesn't include in their iauthentication, the server returns an error message saying "If you want to access this, I'm gonna need to see your credentials". These credentials--the unique authentication-- need to match between the user's stored info and the database's stored info, so the authentication takes places as essentially a conversation between the two parties. Metaphorically, the server is saying "What's the secret password?" and the user get request needs to contain that secret password in order to gain entry. The purpose of this is to prevent a person from being able to access or alter information that they should not be able to access or alter. 
