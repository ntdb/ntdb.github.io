---
layout: post
title:  "Origin + Destination"
date:   2015-01-31
original: "WINTR Blog"
originalurl: "http://www.wintr.us/blog/origin-and-destination"
---

<p>Intro from Ben Winters: <i>Transportation in Seattle is a topic of complaint for the majority of commuters, a byproduct of prosperous times. At WINTR we have a simple belief  that design and technology can be used to solve problems. We created an interactive visualization of personalized experiences in the context of traffic in Seattle. It’s a starting point, something to move the conversation beyond the realm of complaint, to spark a conversation around a solution.</i></p>

<p>Origin+Destination was featured at the 2014 Seattle Interactive Conference and at the Seattle Design Festival.  We developed the installation using a collection of cutting-edge technologies thoughtfully composed to create an engaging, conversational representation of origin, route, vehicle, time, and… destination.</p>

<h5>Say Hello</h5>

<p>It all begins with a text message. Origin+Destination prompts its viewers to add their story to the display by sending their Twitter handle via SMS. We worked with Twilio to make use of the ubiquity of text messaging; the result is an experience that is simple to participate in and easy to enjoy.</p>

<h5>Be Understood</h5>

<p>Once the conversation is started Origin+Destination uses natural language processing techniques (powered by the Natural library) to understand user messages. Each message is compared to a collection of anticipated inputs using Bayes classification and is used by the application to respond to the user in a way that moves the conversation forward.</p>

<h5>Be Found</h5>

<p>When you tell Origin+Destination what neighborhood you call home, it does a quick Google search to geocode your origin. If it knows your destination (like it did for the  attendees at Seattle Interactive Conference in 2014) it calls upon the strengths of the Bing and Google Maps APIs to calculate travel times for walking, biking, transit, or driving (with real-time traffic!) along that route. The appearance of the path from the user’s origin to the pre-determined destination indicates the user’s means of travel and is animated to express travel time in a way that is easy to understand.</p>

<h5>Be Seen</h5>

<p>These efforts to gather information, understand it, and come to a conclusion about it all culminate in the addition of another journey to the Origin+Destination display. We use the animation library Snap.svg to show all of this information in a beautiful and highly performant manner. The visualization is rendered using vector graphics so that it looks great on any device: a mobile phone, a large projection, or on any screen in between.</p>

<h5>Share your Journey</h5>

<p>Each user’s journey is displayed in Origin+Destination with the Twitter handle of its traveller. In addition to allowing the user to easily see their place in the context of the day’s journeys, this also allows them to share their experience on the web. The application is able to recall a specific user’s journey on demand and contrast it with other journeys made by strangers in Seattle on the same day.</p>

<p>Seattle is a city in motion physically, culturally, and economically. Origin+Destination is our expression of just one facet of the city’s movement and the issues that slow it down. Our hope is to motivate creative solutions for these and other issues in order to further Seattle as a city, well designed, in motion.</p>