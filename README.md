# Welcome to the Open Data Hub Bootcamp 2025!
This repo will guide you through the challenge 2, in which you will implement an Hiking route recommender using LLM.

The goal of this bootcamp is to foster our community around the Open Data Hub, to get to know each other, the technology, but also for you to just learn stuff and make friends. This is not a competition, so don't be afraid to make mistakes and try out new stuff. Our Open Data Hub team is there to help and support you.

You will also have an opportunity to present the results to the public at our upcoming event, the Open Data Hub Day

## The challenge
Your goal is to implement a chatbot capable of suggesting an Hiking Route using OpendataDataHub's data given the user question.  

A Visual Interface (web) to let the user interact is a plus!

## Dataset
For this challenge you will need to retrieve data from [**Content API**](https://tourism.opendatahub.com/swagger/index.html).

You can use the [DataBrowser](https://databrowser.opendatahub.com/) to inspect and explore the data visually before diving into the API calls.

Since you will create an Hiking Route Recommender, you are more interested in `ODHActivityPOI` endpoint.  
In particuilar you are looking for all the activities with **tag** `Hiking`.

## Hints
To reduce the number of activities returned and to ensure that all data has the fields you need, we suggest to filter the results to get only those with `source` equals to `idm`.

Get only `active` Hiking routes.

Use `rawFilter` ([documentation here](https://github.com/noi-techpark/opendatahub-docs/wiki/Using-rawfilter-and-rawsort-on-the-Tourism-Api#rawfilter)) to get only the Hiking routes containing informations about the route difficulty in the `PoiProperty`.

Since LLMs have limited input length, retrieve only the fields you need using `fields`.

Start easy supporting only English language!

