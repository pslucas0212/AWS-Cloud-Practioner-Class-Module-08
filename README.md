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

Manage multple AWS accounts - consolidated billing roles up all AWS accounts to one payment
Usage is rolled up to the organization that helps the organization to get bulk discount.  And you can share reserved instances across the organization...

Default number of AWS accounts per organization is 4, but you can request more.

#### Transcript
When you own multiple coffee shops around the city, like we talked about before, each one will have its own expenditures and its own profits. At the end of the day for these coffee shops, they're all owned by the same entity. Because of that, the money is flowing to and from one main account, if there was a coffee machine repair person on call to help fix the coffee machines when they break, that repair person will bill the organization, not the individual coffee shop. 


Okay, let's take that idea and apply it to AWS. A singular company will more than likely have multiple AWS accounts, and as you already learned, you can manage multiple accounts in AWS by using AWS Organizations. One of the lovely features of AWS Organizations is called consolidated billing. At the end of every month, instead of having to pay an AWS bill for every single account, you can roll those bills up into one bill owned by the owner of the organization. This makes it easier to keep track of your bills. You don't get 100 bills, if you have 100 AWS accounts, just like our coffee shop example, if my repair person visited 11 of my coffee shops, repairing coffee makers, they would just make one bill for the billing cycle. So it's easier for the company to manage. 


Same idea with the consolidated billing feature for AWS Organizations. You can still view your AWS bill in an itemized fashion. So you know which accounts spent what, but it all goes into one central location for ease of viewing. There are other benefits of using this feature too. One of them is that the usage for AWS resources is rolled up to the organization level. AWS does offer bulk pricing. Each individual account may only have a small amount of usage, but you can get the bulk discount pricing because of the aggregate across all accounts in the organization. 

In addition, if you have a savings plan in place, or if you are using reserved instances for EC2, it can be shared across AWS accounts in the organization. The best part about this is that the feature is free and easy to use. So it simplifies the billing process, lets you share savings across accounts and doesn't cost you any extra money. Nice.

### AWS Budgets

Want to track costs to stay within a defined budget.  Set customes budgets for costs and usages.  Receive alerts when you are forecasted to meet or exceed budget amounts

AWS Budgets are update 3 times per day. 
#### Transcripts
As you're ramping up your AWS deployments, you probably want to make sure you're not spending an unbudgeted amount. As with most companies, you want to track costs and make sure you keep within your limits. Introducing AWS Budgets. 


Think of a budget for your personal expenses, and you'll be most familiar with AWS Budgets. It allows you to set custom budgets for a variety of scenarios like cost and usage. You will then receive an alert when your costs or usage exceed or are forecasted to exceed your budgeted amount. 


Say my budget was a thousand dollars and I want to be notified when I reach 80% of that amount. Well, with Budgets, you can do just that. That means you can be proactively notified if you're going to exceed your budgeted amount for resources. 


So let me show you what I'm talking about here with a demo. To get started, you navigate to the billing section of your AWS console, click Budgets, then click Create Budget. Choose a type for your budget. I'll pick Cost. Give your budget a name. Enter an amount. Let's say a thousand dollars as I mentioned earlier, and then click Configure Alert. Next, we set an alert threshold. Let's take that 80%, which means we'll get an alert if we've reached 80% of our budgeted amount. Now let's add an email address. Gotta make sure to blur this out, folks. I get enough spam as it is. Now we click Confirm Budget and Create. 


And voila, we have our first budget. How streamlined was that? I think it's safe to say we budgeted our time wisely in that demo.


### AWS Cost Explorer

AWS has a variable cost model.  You pay for what you use and how you use it.   AWS can be used to see how you are spending your money on AWS.  Many resources are taggable by the AWS user.  Tags key-value pair that you attache to AWS services/resources and then you can filter in the AWS cost explorere based on your tag.

#### Transcript
As we have already discussed, AWS has a variable cost model, and you only pay for what you use. You don't have one fixed billed amount at the end of every month. Instead, it fluctuates with the resources you use and how you use them. Because of this cost model, it's really important that you can drill down into your bill and see just how you are spending money. 

AWS has a service called the AWS Cost Explorer, and it's a console-based service that allows you to visually see and analyze how you are spending money with AWS. It will show you which services you are spending the most money on, and it gives you 12 months of historical data, so you can track your spending over time. That way, if you see a bump in spending on, say, EC2 from October to December, you can then use that data to go on and figure out why exactly that happened. 


Let's take a look at AWS Cost Explorer in my own AWS account. You can see I am logged in to the console, and I'm going to type into the search Cost Explorer. From here, I am brought to the Cost Management dashboard, and I will click on Cost Explorer. You can see this is showing me the last six months of cost associated with my account, and it's currently grouped by service. I can change the timeframe it's showing me to eight months and change the data to be grouped by different attributes, and I'll go ahead and select Region. I can group by other attributes as well. 


One important grouping to note is to group by tag. Many resources in AWS are taggable. Tags are essentially user-defined key-value pairs. So you can tag an EC2 instance with a specific project name or a database with the same project name, and then you can come into the AWS Cost Explorer, filter by tag, and see all of the expenses associated with that tag. Cost Explorer also allows you to create custom reports. 


So now what I'm going to do is create a report on the daily cost for the month of January of this year. I'm going to group by service. You can see that the cost of the services is generally the same every day, except that I used more EC2 on some days than others. I can then save this report and come back to it when it is needed. 


So as you can see, Cost Explorer gives you some powerful defaults for reports, but you can build your own custom ones as well. This will help you identify cost drivers and take action when necessary to curb spending. Cost optimization is a priority you should be paying close attention to, and you can use the Cost Explorer to help get you going in the right direction.

### AWS Suspport Plans

Four types of AWS Support
- Basic tier - access customer services 24x7, white papers, AWS trusted advisor, AWS Personal Health dashboard
- Developer tier - Includes everything in basic and you can email support and expect a response in 24 hours
- Business tier - Includes Trusted adivisor and direct phone access to AWS support team with a 4 hour response and 1 hour response if something is down
- Enterprise tier - 15 minute SLA for business critical workloads.  A dedicate Technical Account Manager (TAM)

TAMs is concierge service that comes with Enterprise tier.  And provides additional services like Well-Architected Framework reviews.


#### Transcript
One of the great things about AWS is no matter how big or small your business is, you're never alone. From small startups to large enterprises, private sector, and public, all businesses have support options available that are designed to fit your specific needs. 

To begin with, every customer automatically gets AWS Basic support, no cost at all. Any customer can access support functions like 24/7 access to customer service, documentation, whitepapers, support forums, AWS Trusted Advisor, and the AWS Personal Health Dashboard. It's a personalized view of the health of AWS services and any alerts when your resources might be impacted. These functions are free for everyone, but as you begin to move mission critical workloads into AWS, we offer higher levels of support to match your levels of need. 

The next tier is our Developer tier, which includes everything in the Basic support level. Plus, you can now email customer support directly with a 24 hour response time on any questions you have. And responses of less than 12 hours in case your systems are impaired. This is a great tier for businesses that are experimenting with AWS or setting up tests or proofs of concept. 

Now, as you begin to take production workloads live, we find customers are more successful advancing to the Business tier. Everything in the previous tiers, plus Trusted Advisor now opens up the entire suite of checks for your account. You are given direct phone access to our support team that has a four hour response SLA. If your production system is impaired, and a one hour SLA for production systems down. Additionally, as part of the Business tier, we provide access to infrastructure event management, where for an extra fee, we can help you plan for massive events like brand new launches or global advertising blitzes. 

Finally, for companies running mission critical workloads, we recommend the Enterprise level support. It has everything in the previous tiers. Plus a 15 minute SLA for business critical workloads, a dedicated technical account manager for TAM. They will coordinate access to programs and other AWS experts as needed. 

Let's talk a bit more specifically about the job of a TAM. TAMs are part of the concierge support team that comes with Enterprise level support. They specialize not only in proactively monitoring your environment and assisting with optimizations, but provide infrastructure event management, Well-Architected reviews, and operations reviews. 

What's a Well-Architected review, You ask? Well, keeping it simple, TAMs work with customers to review architectures using the Well-Architected Framework. Architectures are checked against the five pillars of the Well-Architected Framework: Operational Excellence, Security, Reliability, Performance Efficiency, and Cost Optimization. As you can see, the job of a TAM is much more than just handling trouble tickets. AWS Support looks at the customer holistically, not just if they have problems, but how can we help them be successful? 

And that's the mission of AWS Support. To learn more about AWS Support, including pricing structures for the plans, go to aws.amazon.com/premiumsupport.


### AWS Marketplace

One click deployment - procure, deploy and use 3rd party products quickly.  Most vendors allow you to bring your own software to AWS or use their software on a PAYG basis.  Many offer many free trials.

Custom terms and priciing
A private marketplace
Integration into customer purchasing system


#### Transcript

Another huge way that AWS supports your enterprise is through the AWS Marketplace. The AWS Marketplace is a curated digital catalog that streamlines your steps to find, deploy and manage third party software running in your AWS architecture, all while providing a range of payment options, and this allows you to accelerate innovation while rapidly and securely deploying a wide range of solutions, while also reducing your total cost of ownership. 

To help us understand this more, I wanna talk about what the AWS Marketplace brings to the table, and how it can help you improve your speed and agility with AWS. The first key way that the AWS Marketplace helps customers, is that instead of needing to build, install and maintain the foundational infrastructure needed to run these third party applications in the marketplace, customers have options like one-click deployment that allows them to quickly procure and use products from thousands of software sellers right when you need them. 

Now, as you may know, some third party vendors historically have annual contracts for on-premises data centers. You might be wondering, is it the same with an AWS? Well, every vendor can choose what options are available, but almost every vendor in the marketplace will allow you to use any annual licenses you already own and credit them for AWS deployment. But more importantly, as you move forward, most vendors in the marketplace also offer on-demand pay-as-you-go options. These flexible pricing plans give you more options to pay for the software, the way you actually use it without wasted unused licenses weighing down your balance sheets. 

Many vendors even offer free trials or Quick Start plans to help you experiment and learn about their offerings. Because they know just like AWS itself, the best way to see if something works for you is to just run it. Even for large enterprises that are used to negotiating custom rates and discount vendors, well the AWS Marketplace can help. The marketplace offers a number of enterprise-focused features, such as custom terms and pricing, where you can manage custom licensing agreements. A private marketplace, where you can create a custom catalog of pre-approved software solutions that meet your specific legal or security standards. Integration into your procurement systems, and a range of cost management tools just to name a few benefits. To learn more about the AWS Marketplace, go to aws.amazon.com/marketplace.


### Summary

#### Transcript
Well, you've heard a lot about pricing and support, and it's probably a lot more than you initially thought. You learned about the pay-as-you-go nature of using AWS cloud resources. We discussed the difference between on-premises and cloud costs, and we even showed you how you can get your feet wet with the free tier offered with most AWS services. 

We talked about how AWS Organizations can be used and how it can help you with consolidated billing of multiple AWS accounts. We covered AWS Budgets, Cost Explorer. We even explored AWS Console billing, so you could get familiar with it, and then switched gears to talk about the different support models offered on AWS. Very handy if you're looking for assistance on your cloud journey. 

Speaking of assistance, we introduced you to the expansive AWS partner ecosystem so you can find partners to help you with your workloads. And lastly, we touched upon AWS Marketplace if you're looking for click-and-go services.
