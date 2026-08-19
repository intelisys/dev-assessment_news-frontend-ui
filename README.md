# News Frontend UI

## Scenario

Complete a frontend implementation that allows a user to search for news articles. Create a modern and visually
impressive tool that showcases your skills and knowledge of accessibility best-practices, measurability, and
interactivity.

Some of the requirements need you take assumptions for good UX behaviour, and sometimes provide questions for you to think around the functionality.


## Prerequisites

- Register for a free [NewsAPI API Key](https://newsapi.org/register) for use as a data source within your project
  submission

## Requirements
1. Retrieve news data from [NewsAPI](https://newsapi.org/docs) using the API key you got above
   - Allow the user to configure an API key through a JavaScript function exposed to dev tools console or page input rather than requiring a committed secret. Never commit a real API key.
   - Provide useful loading, empty, error, and rate-limit states.
2. Include a text input field for searching articles by keyword
   - Show recent searches in search suggestions when the search input is focussed.
   - Should you send the API request on every typed letter?
   - What happens when user refreshes the page when they are on search page?
   - How should the API behave when requests overlap, the network fails, NewsAPI rate-limits the client, or an older response arrives after a newer search?
3. Display results with the article image, title, and description
   - Is simple loader better here or skeleton loading state is better?
4. Display a Read More button linking to the full article.
   - Show an interstitial popup warning the user that they are going to an external website if the URL is not matching the current host url. If they choose yes, then redirect them to the expected URL.
   - We don't want to lose the ability to see the link, so don't avoid using the `a` tag.
   - How will the interstitial work, if user opens the link in new tab (by doing middle click or Right Click -> Open link in new tab)?
   - Is it better to implement an "Always remember" or "Trust this website" to reduce number of interstitial popups?
5. Provide functionality for sorting results based on popularity, relevancy, publish date, or none.
   - What happens to sorting when user refreshes the page?
6. Show a small clock that displays the correct current time even if local system clock is inaccurate.
   - Use (time.now)[https://time.now/developer] API to sync deterministic time on the basis of user's timezone
   - What happens when the browser tab is not in focus for long time (like 30 min)?
7. Add some unit tests for important behavior.

## Bonus Features
You can choose to implement 1-2 features from this that you like:

1. Use relative time for the article's published times, e.g. 3 min ago, Yesterday 2 PM.
   - Where relative times work best for News articles (e.g. Last week vs Thursday 3PM).
   - How will the values update if the page remains open for long durations (like a whole day) in background?
2. Give an option to the user to mark a news source as favourite.
   - If a favourite news source appears in search list, it should show before the news from other sources
3. If user has visited the main article for a news item from the "Read more" link, it should show "Visited" tag for such news items

Make sure you implement all the features' main problem statement. To address the questions asked in the requirements, you can implement the functionality if the time allows it, so prioritize the work and document any items you were not able to complete.

## Parameters

- Build, organize, and commit your code (via git) as if you are working on a production project
- Login credentials or user management is not a requirement of this assessment. There is no backend or DB service needed to implement the assessment. For any kind of information persistance, you can use the browser to store it.
- You may leverage any boilerplate or starter app code to help bootstrap your project
- Modern React is expected

## Delivery Timeline

It is expected that you will spend no more than 4 hours total on this assessment but we will provide a preferred
delivery date, exceeding the deadline is acceptable but will be considered. You may spend more or less time as
you feel appropriate to complete the assessment.

Prioritize the areas of development you feel are most important and directly address the requirements. If your
submission is not complete after one week, submit what you have.

## AI Agent Policy

Use of AI in the submitted assessment is allowed, but care should be taken in doing so. Be prepared to explain your
approach or thought process in all lines of submitted code. Submissions that are overtly "vibe coded" or heavily
contributed by an agent without justification may result in the candidate being disqualified. Use your best judgment.

## Submission

Your submission must include:

- All files necessary to run your project should be commited as you would for a production application
- A readme with instructions on how to build and run your project

Push the solution to a public GitHub repository and provide the link via email to the contact who provided this
assessment.

## Disclaimer

This project is for candidate evaluation purposes only.  No ownership rights are granted herein.  Code provided as part
of this test will not be used as part of any commercial or personal applications and will be deleted following
evaluation.  This project is not intended to be defined as work for hire and will include no compensation for time
spent.
