---
layout: post
title:  "Let me Audit Your Test Suite"
description: "I'd love to audit/profile your test suite, and then make it faster!"
date:  2021-05-13 06:00:00 -0700
crosspost_to_medium: false
categories: [services]
tags: [testing, profiling]
permalink: let-josh-audit-and-improve-your-test-suite
image: /images/title_image.jpg
github_issue_id: 7
---


## Background

A few weeks ago I was talking with a very experienced engineer about their test harness, and how (un)happy they were with how long it took the test harness to run. I said 

> hm, I wonder if I could spend an hour or two on it and get it running faster. 

He can't be adding random people to his client's repositories, so he suggested I just ask Twitter for _their_ RoR applications, to get practice on a lot of different applications. 

So I tweeted some thing: 

<blockquote class="twitter-tweet"><p lang="en" dir="ltr">Strongly recommend you charge at least $1,000 to signal you&#39;re serious and know what you&#39;re doing. <br><br>&quot;I gave access to our source code to an extremely cheap contractor&quot; is not something most folks want to say to their boss.</p>&mdash; Ben Orenstein (@r00k) <a href="https://twitter.com/r00k/status/1393124330461143042?ref_src=twsrc%5Etfw">May 14, 2021</a></blockquote> <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script> 

It was a great suggestion. And thus this page was born.

_update from the future: As you might not be surprised to hear, I got some customers, and prices have gone up!_

---------------------

I'm a bit of an obsessive about how long it takes to run tests.

Slow tests have such a cost to you, your team, and your company. (And have cost _me_, _my_ teams, and the companies I've worked for lots of time, hassle, and payroll)

I've been on teams where the tests take 30 seconds, and I've been on teams where the tests take 45 minutes.

I'm not going to engage in _shaming_ anyone for having a slow test suite. I'd like to simply teach them how to profile/benchmark their own tests, and then make some tactical, selective fixes, and immediately get faster tests!

_I'm going to write a companion guide, documenting as much of what I can document as I can. Want to get the`Speed Up Your RoR Tests` guide when it's done? Drop your email below 👇. [here's a preview](https://www.intermediateruby.com/how-to-audit-and-improve-your-ruby-rails-test-suite)_

<script async data-uid="518bab5f60" src="https://josh-thompson.ck.page/518bab5f60/index.js"></script>

## What you'll get

Because I'd like to get exposure to many different test suites on different applications, and get practice with profiling them and making the them faster, I'd like to do this on _your_ application! 

Critically, however, _I might not be able to make your tests faster_, but I'll certainly try, and I'll give you great starting points that your team can continue to work on. 

If your tests take 45 minutes, I don't know that they'll ever take just one minute, but think of how nice it would be to cut that time by twenty or thirty minutes!

If your tests take 5 minutes, how nice would it be if they took just 1.5 minutes?

I'd like to help you, and get some practice doing this on a wide variety of applications, so I can build a guide to help other engineers figure this all out for themselves!

So, hit the "buy now" button to book an audit. Once payment is complete, I'll reach out via email, and we'll get things going!

I think it'll be a good bit of fun. 😀

## Purchase Now

<!-- Load Stripe.js on your website. -->
<script src="https://js.stripe.com/v3"></script>

<div class="stripe_button_container">
<!-- Create a button that your customers click to complete their purchase. Customize the styling to suit your branding. -->
  <button class="stripe_button"
    id="checkout-button-sku_JTcq1iheI2La2N"
    role="link"
    type="button">
    Buy Now ($4900)
  </button>
</div>
<div id="error-message"></div>

<script>
(function() {
  var stripe = Stripe('pk_live_sPYviTcMAWXUxiZKnVtA1zW300d6I1ltcW');

  var checkoutButton = document.getElementById('checkout-button-sku_JTcq1iheI2La2N');
  checkoutButton.addEventListener('click', function () {
    /*
     * When the customer clicks on the button, redirect
     * them to Checkout.
     */
    stripe.redirectToCheckout({
      lineItems: [{price: 'sku_JTcq1iheI2La2N', quantity: 1}],
      mode: 'payment',
      /*
       * Do not rely on the redirect to the successUrl for fulfilling
       * purchases, customers may not always reach the success_url after
       * a successful payment.
       * Instead use one of the strategies described in
       * https://stripe.com/docs/payments/checkout/fulfill-orders
       */
      successUrl: window.location.protocol + '//intermediateruby.com/success',
      cancelUrl: window.location.protocol + '//intermediateruby.com/canceled',
    })
    .then(function (result) {
      if (result.error) {
        /*
         * If `redirectToCheckout` fails due to a browser or network
         * error, display the localized error message to your customer.
         */
        var displayError = document.getElementById('error-message');
        displayError.textContent = result.error.message;
      }
    });
  });
})();
</script>

## Enterprise Options

If your company is too big/process heavy to support this exact mechanism (an easy $4900 charge + github access), there's other working arrangements we can explore, but it's still best to funnel through the $4900 audit and profile option, and *then* explore additional work arrangements

--------------------

## FAQ

### This seems too good to be true. $4900 for faster tests, and all that earned-back confidence and productivity?

Well, it really could be too good to be true. I only have room to do a few of these at a time, and often-enough the audit/fix turns into additional work, further limiting my availability for other customers.

You're normally paying that much every week for each of your engineers who are currently making pull requests, running tests, and overall trying to build your product as fast as possible - outsource the stress, project management, pointing, and stress for making your tests faster to me, who _loves_ making things faster.

I'll share my learnings with your engineers, so some of them might keep the performance mindset going, even after my work, and this will be an investment that keeps on generating returns



### What makes for a "good fit" for this service?

- **Your tests are in Ruby/Rails** I'd like to work on _just_ Ruby and/or Rails test suites. I don't want to work on elixir/javascript/java/whatever codebases.
- **you can add me to the repository where your tests live.** We can get a SoW and NDA in place easily enough, but ultimately the work will look like adding me to the necessary github repository and CircleCI, and I'll take it from there. 
- **You're willing to talk with me about it a bit** I might have some questions, and might open up a GitHub issue, or DM you in Slack|Twitter|Discord|whatever. 
- **You're not obsessing too much about this** If you're really nervous about parting with your money need me to turn your payroll into a few million dollars of valuation, maybe it's not a good fit right now. Once I've iterated on this a few times, it'll be a much more robust service/offering, and _then_ we should talk! Punch your email in below, and you'll get updates as I go!

<script async data-uid="518bab5f60" src="https://josh-thompson.ck.page/518bab5f60/index.js"></script>


### What if you don't make my tests go faster?

I'll give you half of the money back! (but not all of it, of course. My time has value)

### $4900? Isn't that a little cheap?

It is! A normal full-time engineer might cost you $15-25k/month, and it's time consuming for everyone to find and hire that person. I offer dramatically reduced effort, without displacing any of the work you/your team already has on deck. 

I don't think I'll leave the cost so low for long, and it's been even lower in the past. 

### $4900? Isn't that a little expensive?

The average full-time software developer costs the company in the ballpark of $15-20k/mo, and then needs to be interviewed, hired, onboarded. All of that costs money, of course, and lots of time.

Buying this productized service at such a low cost is the kind of thing that you'll record as 'an easy win for the quarter'. Every engineer will be happy to have faster tests, _and_ to have not gotten performance work dropped in their lap at an inconvenient time. 

I have an odd interest in performance work, and find it satisfying, and you get access to all the assorted experience and knowledge I've gained, doing this for many different companies/codebases.

Tl;Dr; I'm basically giving this service away.

### I've got a super slow test suite, and I'd love for you to guaranteed that it'll be a lot faster when you're done

I cannot guarantee it, but I can promise that you (and I!) will learn a lot through the process. [here's some of what I learned and achieved in the past](https://www.intermediateruby.com/how-to-audit-and-improve-your-ruby-rails-test-suite)

### Can I get that guide you're going to write when it's done?

Absolutely!

Drop your email below, and I'll notify you when this project is done!

<script async data-uid="518bab5f60" src="https://josh-thompson.ck.page/518bab5f60/index.js"></script>

(Or you can [follow me on Twitter](https://twitter.com/josh_works), or [sponsor me on GitHub](https://github.com/sponsors/josh-works) for between $1 and infinite dollars per month.)

### I've got more questions. What to do?

Leave a comment below. Hit me up on twitter. Email me at `josh@intermediateruby.com`.
