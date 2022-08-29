# Pricing and Support

[AWS Cloud Practitioner Home](https://github.com/pslucas0212/AWS-Cloud-Practioner)

### Introduction


#### Transcript
Well, now that Morgan is the owner of the coffee shop, she probably has a lot of logistics to worry about as well as all the costs that come with this added responsibility. Costs like the building lease, the tables, the cost of the employees, of course. What about taxes? What about power, and heating, and air conditioning? And what about the groundskeepers who keep the outside looking so nice? And a much more important question is, how much is it going to cost next month to keep the store open? There's really a lot of moving parts. 


We certainly could get a good ballpark of how much it costs per month and just estimate what next month might be, knowing that it's about to start the busy season. In order to get the exact amount, we need to know how much each item costs and how many of them we're planning to use next month. Put them in a table and that'll calculate the prediction. Done. 


Now, we might also be asking questions about what it might cost to move to an entirely different city, and what would be the cost differential there? All of these questions are exactly the kinds of questions that we're going to answer in this next section, as we talk about pricing and support. And spoiler alert, AWS provides a lot of free tools to help you plan and analyze your budgets for your AWS environments. Let's dive on in.

### AWS Free Tier

Three types of offers:
- Always Free.  Lambda allows 1 million free invocations per month as of March 2020.  Free tier does not expire.
- 12 months to try out a service.  S3 free for 12 months with 5GB
- Trials - Some services offer a short term trial... AWS Lightsail deploy ready made application stacks.  1 month trial up to 750 hours o usage

Sagemaker, dynamoDB, etc.   Approximately 60 services make up the free tier.

#### Transcript
So you've created a brand spanking new AWS account and want to get started, but you're worried about exhausting your credit limit. Well, don't worry. If you're looking to try out some AWS services, you might be able to try them out under our Free Tier. 


Depending on the product you're looking at, the Free Tier offers three different ways to try out a service. Number one, always free. That means a service is available to all AWS customers and the Free Tier does not expire. Number two, 12 months free. That means you have 12 months to try out a service following your initial signup date to AWS, so the date you created your AWS account. And number three, trials. Some services offer a short-term free trial, and then they expire after that period ends. 


Simple enough, right? Let's illustrate with a few examples. Let's take AWS Lambda, our serverless compute option. As of March 2020, it allows for one million free invocations per month. That means if you stay under one million invocations, it's always free. This Free Tier never expires. Another example is S3, our object store service. It's free for 12 months for up to five gigs of storage. Thereafter, you'll incur a cost. Great for trying out a static website on S3, I might say. And the last example is Lightsail where you can deploy ready-made application stacks. We offer a one month trial of up to 750 hours of usage. That's a pretty decent amount to deploy and test a WordPress blog. I mean, who knows, maybe you wanna show people your smoothie recipes. 


But before I digress, some other services that qualify under the free tier are SageMaker, Comprehend Medical, DynamoDB, SNS, Cognito, and so much more. If you want to see the full list of 60 or so services, please check out our Resources section. Happy exploring of the Free Tier.

### How AWS Pricing Works
- Pay for what you used
- Pay less when you reserve
- Pay less with volume-based disounts when you use more

Use the AWS pricing calculaor to estimate cost for your use cases

### Billing dashboard

AWS Billing & Cost Management Dasbhoard
You can see current montly spend
Last month spend
Top 3 service spends

Click bills to specifically region usage as well as global services

#### Transcript
Hey there, AWS aficionados. Are you like me and curious about billing information of your AWS account? Well, let's walk through a demo so you know where to go. 


As you can see, I'm already logged in and now we're gonna search for billing and click the option that shows up. And boom, with that, you already have some useful information. You can see your month-to-date spend on the right-hand side with the top services being used. Below on the left is the last month, current and forecasted amounts. Below that is the top Free Tier services by usage. You even get the percentages of your month-to-date usage. Nifty, right? 


If we scroll up, you can see you have access to other billing tools, such as Cost Explorer, Budgets, along with a few others. You also get access to your bill itself. So let's click Bills. Now, you can see we have the services that we are paying for, and if we expand them, we get to see the costs broken down by region. And for global services, we see them broken down as such. For example, if I click Route 53, you can see it's a global service and is broken down that way. 

And there you have it, a simple way to check out what you're spending on each service in AWS. Thanks for joining us.

### Consolidated Billing

#### Transcript
When you own multiple coffee shops around the city, like we talked about before, each one will have its own expenditures and its own profits. At the end of the day for these coffee shops, they're all owned by the same entity. Because of that, the money is flowing to and from one main account, if there was a coffee machine repair person on call to help fix the coffee machines when they break, that repair person will bill the organization, not the individual coffee shop. 


Okay, let's take that idea and apply it to AWS. A singular company will more than likely have multiple AWS accounts, and as you already learned, you can manage multiple accounts in AWS by using AWS Organizations. One of the lovely features of AWS Organizations is called consolidated billing. At the end of every month, instead of having to pay an AWS bill for every single account, you can roll those bills up into one bill owned by the owner of the organization. This makes it easier to keep track of your bills. You don't get 100 bills, if you have 100 AWS accounts, just like our coffee shop example, if my repair person visited 11 of my coffee shops, repairing coffee makers, they would just make one bill for the billing cycle. So it's easier for the company to manage. 


Same idea with the consolidated billing feature for AWS Organizations. You can still view your AWS bill in an itemized fashion. So you know which accounts spent what, but it all goes into one central location for ease of viewing. There are other benefits of using this feature too. One of them is that the usage for AWS resources is rolled up to the organization level. AWS does offer bulk pricing. Each individual account may only have a small amount of usage, but you can get the bulk discount pricing because of the aggregate across all accounts in the organization. 

In addition, if you have a savings plan in place, or if you are using reserved instances for EC2, it can be shared across AWS accounts in the organization. The best part about this is that the feature is free and easy to use. So it simplifies the billing process, lets you share savings across accounts and doesn't cost you any extra money. Nice.


