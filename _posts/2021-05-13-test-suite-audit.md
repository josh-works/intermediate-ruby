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

I'd like to do this 'Rails app test suite benchmark/profile/optimize on _your_ application! 

If your tests take 45 minutes, think of how nice it would be to cut that time by 30%. I don't promis results, but it's easy to imagine the benefits of faster tests. Your developers will thank you, and you'll feel a bit more confident about the deploy pipeline. Fail fast and all. 

If your tests take 5 minutes, how nice would it be if they took just 2 minutes?

I'd like to help you, and get some practice doing this on a wide variety of applications, so I can build a guide to help other engineers figure this all out for themselves! [This guide lives here for now](https://www.intermediateruby.com/how-to-audit-and-improve-your-ruby-rails-test-suite)

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


--------------------

## FAQ

### How long will it take for you to finish?

Once I'm added to your organization's github repo, and provisioned with enough access to run the tests locally, I'll do my work, and will open a PR fairly quickly in the process where we'll land the benchmarking & profiling results, fixes, etc. 


### How'd you arrive at the price? Aren't you supposed to have tiers?

Yep, some pricing strategies say 'have tiers'. Instead I'll anchor the price with the cost of hiring/onboarding a full-time engineer, and then getting them started with the bug-fixing, then feature work. You've got urgent work for your team, no one is thrilled to put one of them intensely on 'developer happiness' projects.

So, even after spending $60,000 in payroll, you might still not find it easy to get some performance work done. Big app or small, many engineers or three, there's a strong business case to be made. I'd love to have a phone call (actuall phone calls/whatsapp calls preferred) to discuss it more. I've found that a single phone conversation is a great use of time, then we can kick it off and i can take it from there. 

Theoretically I could offer the work for less, I suppose, and I have done so in the past, but the price has gone up, probably will keep doing so. The 'cheaper' option would be [a small written guide](https://www.intermediateruby.com/how-to-audit-and-improve-your-ruby-rails-test-suite). The more expensive option, lets call it $10k, a reasonable and round figure. 

### Have you done non-test performance work?

Yes, that's kinda where I got started, then moved sideways into tests. 

A few years back, I gave a talk around rails app performance things, titled "Move Slow And Improve Things"

The group laughs 8 times in the first 2.5 minutes, i'm proud. [It might be worth the click](https://www.youtube.com/watch?v=992Uyrheo24).

<iframe width="560" height="315" src="https://www.youtube.com/embed/992Uyrheo24" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture; web-share" allowfullscreen></iframe>

### $4900? Isn't that a little expensive?

The average full-time software developer costs the company in the ballpark of $15-20k/mo, and then needs to be interviewed, hired, onboarded. All of that costs money, of course, but also time and energy, from quite a few different people.

Buying this productized service at such a low cost is the kind of thing that you'll record as 'an easy win for the quarter'. Every engineer will be happy to have faster tests, _and_ to have not gotten performance work dropped in their lap at an inconvenient time. 

I have an odd interest in performance work, and find it satisfying, and you get access to all the assorted experience and knowledge I've gained, doing this for many different companies/codebases.

tl;dr I'm basically giving this service away.

### I've got a super slow test suite, and I'd love for you to guaranteed that it'll be a lot faster when you're done

I cannot guarantee it, but I can promise that you (and I!) will learn a lot through the process. [here's some of what I learned and achieved in the past](https://www.intermediateruby.com/how-to-audit-and-improve-your-ruby-rails-test-suite).

If the test suite is so big it can only be run on circleCI, for example, that still can be made better, and we can get your monthly credit burn a bit lower. 

### Can I get that guide you're going to write when it's done?

Absolutely!

Drop your email below, and I'll notify you when this project is done!

<script async data-uid="518bab5f60" src="https://josh-thompson.ck.page/518bab5f60/index.js"></script>

(Or you can [follow me on Twitter](https://twitter.com/josh_works), or [sponsor me on GitHub](https://github.com/sponsors/josh-works) for between $1 and infinite dollars per month.)

### I've got more questions. What to do?

Leave a comment below. Hit me up on [twitter](https://twitter.com/josh_works). Email me at `josh@intermediateruby.com`.


