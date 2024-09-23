---
title: "Structuring an API Document"
description: "This article offers a comprehensive guide on structuring API documentation for beginners. It explains the key sections every API document should include, such as the introduction, quick start, authentication, status/error codes, and rate limiting. Each section is designed to help developers understand how to navigate and use the API effectively."
summary: "The article covers the fundamental structure of an API document, emphasizing the importance of organization and user experience."
date: 2024-09-16T07:07:07+01:00
lastmod: 2024-09-16T16:04:48+02:00
draft: false
menu:
  docs:
    parent: ""
    identifier: "structure-6a1a6be4373e933280d78ea53de6158e"
weight: 1
toc: true
seo:
  title: "Structuring an API Document" # custom title (optional)
  description: "This article offers a comprehensive guide on structuring API documentation for beginners. It explains the key sections every API document should include, such as the introduction, quick start, authentication, status/error codes, and rate limiting. Each section is designed to help developers understand how to navigate and use the API effectively." # custom description (recommended)
  canonical: "" # custom canonical URL (optional)
  noindex: false # false (default) or true
---

An API document is more than a collection of pages—it's the complete guide to your product's API.

Every page in this document needs to capture a specific aspect of the API, ensuring that users have all the details they need to maximize its potential.

The structure of your API document isn't just about organization; it's about creating a user-friendly experience for your users.

It's crucial to think carefully about how each page is arranged because this will guide users' interactions with your API.

Imagine starting with an error handling page before giving users a proper introduction or overview of the API.

In this section, you'll learn how to structure API documentation, explore the significance of each page, and determine what its content should be.

## **Introduction (Product Overview)**

The introduction page of your API is your chance to make a solid first impression. It's where you provide a soft landing for your users, giving them a clear and concise overview without overwhelming them with details.

In API documentation, you often don't have the luxury of long-winded stories or paragraphs, so this is the page where you need to grab attention quickly.

On this page, you'll provide a high-level overview of the API, its purpose, and how it can be used. The goal is to give developers a solid understanding of what they can achieve with the API and why they might want to use it.

Your introduction page typically includes the following sections:

1. **Overview**: This briefly describes the API, its core functionality, and the problems it solves. It sets the stage for the rest of the documentation.

2. **Key features**: Highlight the API's most important features or capabilities, helping developers quickly determine if it meets their needs.

3. **Use cases**: Provide examples of applying the API in real-world scenarios. This helps developers visualize its potential.

4. **Getting started**: Include a link to a quick guide or steps to help developers use the API immediately. This might cover setup instructions, authentication details, or links to more detailed sections.

5. **Versioning and updates**: If the API has recently been updated, include information about the current version. This keeps developers informed about the API's lifecycle.

As a tip for creating this page, please stick to the company's tone and voice, as it sets the foundation for the rest of the documentation. If you're unsure, aim for a friendly tone that's easy to follow, avoiding vague or overly complex language.

Consider adding images or videos about the product to enhance the page's look and feel. A well-designed introduction page can set the right tone for the entire documentation.

{{< callout context="tip" title="For inspiration, check out the introduction page of this web3 product, [Bitpowr](https://docs.bitpowr.com/reference/api-reference), or this video game API, [RAWG](https://rawg.readme.io/reference/overview):" icon="rocket" >}}
{{< /callout >}}

<img src="https://paper-attachments.dropboxusercontent.com/s_EDD9ADFB86920F498AB507D4AA462F35DADB64AD2D2C85E101246DF4DE91B194_1724569494303_RAWG-intro.png" alt="clear image" width="100%">

## **Quick Start**

After showcasing all the incredible things developers can do with your API on the introduction page, it's time to put all that talk into practice.

This guide is all about action. Your goal is to lead developers through the steps to make their first API call quickly and efficiently. The name says it all: it's a quick-start guide, so keep the focus on code; there is no need for stories.

Your job in this guide is to take the user by the hand and walk them through a series of steps to achieve a tangible result. Think of it like writing your first "**hello world**" program—simple, direct, and concise.

To be effective, this guide must be as self-contained as possible. This means it should include everything the developer needs to get that first successful response from your API without having to hunt for information elsewhere.

Below are some key elements to include in the quick start guide:

1. **Prerequisites**: What does the developer need before they start? This could include tools, environment setups, or specific API keys.

2. **Authentication**: Clearly explain how to authenticate with the API. This is often the first hurdle, so make it easy to understand. This process is usually lengthy and can be found on another page. In that case, please provide a link to it.

3. **Step-by-Step Instructions**: Break down the process into clear, actionable steps with code snippets that developers can copy and paste. Each step should build toward a final goal.

4. **Example Request and Response**: Provide a real example of an API call, including the request and the expected response. This helps developers see what success looks like.

5. **Error Handling**: Briefly mention what to do if things go wrong. You don't need to go into detail here, but pointing out common pitfalls can save a lot of headaches.

As a tip, you want to make this page as brief as possible, so select an endpoint that's easy to call and has a high use case for this guide.

{{< callout context="tip" title="The [Movie Database API](https://developer.themoviedb.org/reference/intro/getting-started) provides a good example of what a quick start guide should look like:" icon="rocket" >}}
{{< /callout >}}

<img src="https://paper-attachments.dropboxusercontent.com/s_EDD9ADFB86920F498AB507D4AA462F35DADB64AD2D2C85E101246DF4DE91B194_1724569648391_TMDB+quick+start.png" alt="clear image" width="100%">

## **Authorization/Authentication**

Before users can interact with any endpoint on your API, they need to authenticate themselves, typically using an API key.

While API keys are a popular choice for authentication, they're not the only method available.
Before discussing how this page should be structured, you need to understand what authentication is and other means of authentication.

### **What is Authentication?**

Authentication is all about verifying who someone is. When a user wants to access your API, they need to prove their identity.

This is where authentication methods like API keys, OAuth, or HMAC come into play. It's the first line of defense, ensuring that only legitimate users can interact with your API.

### **What is Authorization?**

Authorization, on the other hand, determines what an authenticated user is allowed to do. Once a user is authenticated, authorization defines their level of access—what resources they can use, what actions they can perform, and what data they can interact with.

### **Their differences?**

Authentication asks, "Who are you?" Authorization asks, "What are you allowed to do?" While these concepts are closely related, they serve different purposes.

Think of authentication as the lock on the front door and authorization as the rules for what rooms someone can enter once inside.

### **Authentication methods**

Authentication isn't one-size-fits-all. Below are some common methods of authenticating a user:

#### API Keys

API keys are like a unique password for your API. They're simple and easy to use, making them a go-to choice for many developers.

However, while convenient, they may not offer the highest level of security, especially if not handled properly.

#### OAuth

OAuth is a more robust and secure method of authentication, particularly popular in scenarios where users need to grant third-party apps access to their data without sharing their actual credentials. It's a bit more complex but offers greater flexibility and security.

#### HMAC

Hash-based Message Authentication Code (HMAC) adds an extra layer of security by combining a secret key with the message itself to generate a unique signature.

This method ensures that the message hasn't been tampered with and comes from a legitimate source.

### **How to structure this page**

When structuring the authentication/authorization page, you want to ensure it is clear and straightforward.

Therefore, you should include the following:

1. **The type of authentication method used**: Clearly state which authentication method your API uses, whether it's API keys, OAuth, HMAC, or another method. Provide a brief explanation of why this method was chosen. Do well to leave it at a high-level description for increased security.

2. **The steps to get authenticated**: Guide the user through the steps they need to take to authenticate themselves. Include setup instructions, such as where to obtain keys or tokens and how to use them in API requests.

3. **Error codes relating to authentication issues**: List and explain the error codes developers might encounter when authentication fails. Include tips on how to resolve these issues.

4. **How to handle authentication information**: Offer best practices for securely handling authentication credentials. This might include advice on storing API keys, using environment variables, or securing OAuth tokens.

5. **Expiry rate**: Inform users if and when their authentication credentials will expire and what steps they need to take to renew them.

{{< callout context="tip" title="The [Interswitch API](https://docs.interswitchgroup.com/docs/authentication) docs provides an excellent example of an authentication page." icon="rocket" >}}
{{< /callout >}}

<img src="https://paper-attachments.dropboxusercontent.com/s_EDD9ADFB86920F498AB507D4AA462F35DADB64AD2D2C85E101246DF4DE91B194_1724569682732_interswitch-auth.png" alt="clear image" width="100%">

## **Status and Error Codes**

Status and error codes are essential elements in an API's response. These codes, embedded in the response header, serve as a communication tool between your API and the developer, indicating the status of a request. For example, you'll see a 200 code if everything went smoothly. If there's an authentication issue, you'll get a 403 code instead.

While many of these codes are standardized across APIs, it's crucial to dedicate a page detailing them, especially those unique to your API. This page is a central reference, helping developers understand what each code means and how to handle it.

For endpoints that require a specific explanation of an error, it's good practice to provide a brief description within the endpoint's documentation and link it back to this general page for more context.

### **Documenting this page**

When documenting this page, the developers usually supply the codes associated with each endpoint. However, it's a good idea to play around with the endpoints yourself to observe the codes in action. This hands-on approach ensures accuracy and gives you a deeper understanding of how these codes function within your API.

Double-checking is critical because these codes are often the developer's first and only clue when something goes wrong. They play a pivotal role in troubleshooting, and having precise, well-documented error codes can make the difference between a frustrating debugging session and a quick fix.

{{< callout context="note" title="To document this page effectively, organize the codes and their descriptions in a table. Below is an example:" icon="rocket" >}}
{{< /callout >}}

| **Status Code** | **Description**                                                                                  |
| --------------- | ------------------------------------------------------------------------------------------------ |
| 200             | OK - The request was successful.                                                                 |
| 201             | Created - The resource was successfully created.                                                 |
| 450             | Custom Error - A specific error unique to your API that requires detailed troubleshooting steps. |
| 460             | Validation Error - Input data did not meet the required specifications.                          |
| 499             | Client Closed Request - The client closed the request before the server could respond.           |

{{< callout context="tip" title="An excellent example of an errors and status codes page can be found on the [Paystack API documentation.](https://paystack.com/docs/api/errors/)" icon="rocket" >}}
{{< /callout >}}

<img src="https://paper-attachments.dropboxusercontent.com/s_EDD9ADFB86920F498AB507D4AA462F35DADB64AD2D2C85E101246DF4DE91B194_1724569804556_paystack-errors.png" alt="clear image" width="100%">

## **Rate Limiting**

The rate limiting page explains how many requests a user can make to the API in a specific period, like per minute or hour.

It's an important part of API docs because it helps developers understand how to use the API without issues, such as getting blocked for making too many requests.

Many companies offer different rate limits based on their pricing tiers. For example, a free tier might have stricter limits, while a commercial plan offers more flexibility, allowing users to make more requests. This gives developers options depending on their needs and budget.

### **How to document this page**

You should include the following information in your rate limit page:

- **Limits**: State how many requests are allowed and in what time frame.

- **Time frame**: Specify the period for the limit, like per minute or hour.

- **Response codes**: Explain what happens if the limit is exceeded, including the specific error codes, like `429 Too Many Requests`.
- **Headers**: List any headers that show the current rate limit status, like `X-RateLimit-Limit` and `X-RateLimit-Remaining`.

- **What happens if you exceed the limit**: Describe the consequences, like being blocked or waiting before making more requests.

- **Tips for staying within limits**: Provide advice on avoiding hitting the limit, like spacing out requests or using caching.

- **Exceptions**: You should also mention if different endpoints or user levels have different limits.


{{< callout context="tip" title="[X (Twitter)](https://developer.x.com/en/docs/x-api/rate-limits) provides a detailed API rate limit section for inspiration. If you scroll further down this page, you can see how they structured the rate-limiting information based on tiers in tables." icon="rocket" >}}
{{< /callout >}}

<img src="https://paper-attachments.dropboxusercontent.com/s_EDD9ADFB86920F498AB507D4AA462F35DADB64AD2D2C85E101246DF4DE91B194_1724570007110_x-rate-limit.png" alt="clear image" width="100%">

{{< callout context="note" title="Assignment" icon="outline/info-circle" >}}

Document the [Petstore API](https://petstore.swagger.io/) using Postman. Pay attention to the API's structure as explained in the course module and provide detailed descriptions and examples where necessary.

{{< /callout >}}