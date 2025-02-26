# Configuring trailing context settings on frontends

Have a general front-end architecture request and thought this would be the place to come for advice. 

## Use Case

I have a few assistants set up for data processing and writing reformatting type workflows. 

For example, something like "when the user provides a screenshot, extract it to CSV, use this exact template."

For convenience, and because I've created quite a lot of these, I'm using Open Web UI for frontend.

Even though these tasks are much more instructional than conversational, the chat interface still comes in extremely handy because I can use it to quickly prompt corrections and edits when required.

## The Problem

The correct behaviour for instructional tasks like this, I assume, is to create a new conversation for every request. However, this can be quite inconvenient if you're running these kind of light data processing tasks frequently. 

## What Would Be Great

As a general frontend feature, two implementations would be majorly helpful:

1) Enforced single turn threads. This option would negate the ability to provide follow up instructions unless some additional logic could be configured. But it still might have its uses. Under this structure, no context is retained within the thread and every follow-up prompt is treated as if it were the initial prompt. In such a case, the "thread" or "conversation" provided on the frontend would be just a convenience and the model would actualy have no memory of previous turns.

2) Much more useful and for many more use-cases: The ability to specify the trailing context retention depth within a conversation. In other words: how many prior tokens should we go back when sending the next one?  

The latter would be extremely helpful when configuring agent type workflows that might begin with a long block of code and that might not be helpful in subsequent turns. 

My question in general terms is whether there are any standard front-end parameters that can be used to enforce this kind of preference or whether you have to work with what the API provides. 

Many thanks in advance for any pointers!








