# News Frontend UI

## Scenario

Complete a frontend implementation that allows a user to search for news articles. Create a modern and visually
impressive tool that showcases your skills and knowledge of accessibility best-practices, measurability, and
interactivity.

Some of the requirements require assumptions about good UX behavior. You submission will be graded on the best
practices and standard UX decisions you make, as well as how those decisions shape the application architecture.
Prioritize a maintainable, accessible, and reliable experience, and document important assumptions and trade-offs in your submission.


## Prerequisites

- Register for a free [NewsAPI API Key](https://newsapi.org/register) for use as a data source within your project
  submission

## Requirements
1. Retrieve news data from [NewsAPI](https://newsapi.org/docs) using the API key you got above
2. Include a text input field for searching articles by keyword
   - Show recent searches in search suggestions when the search input is focussed.
   - Use an appropriate strategy for request timing, URL state, overlapping requests, network failures, limits, and stale responses.
3. Display results with the article image, title, and description.
4. Display a Read More button linking to the full article.
   - Show an interstitial popup warning the user that they are going to an external website if the URL is not matching the current host url. If they choose yes, then redirect them to the expected URL.
   - Preserve standard link behavior and accessibility, including the ability to open the link in a new tab.
   - Consider an appropriate experience for repeated visits to a trusted external website.
5. Provide functionality for sorting results based on popularity, relevancy, publish date, or none.
   - Preserve the selected sort when the page is refreshed or shared where appropriate.
6. Show a small clock that displays the correct current time even if local system clock is inaccurate.
   - Use the [time.now API](https://time.now/developer) to sync deterministic time based on the user's timezone.
   - Keep the displayed time accurate when the browser tab is not in focus for an extended period.
7. Add some unit tests for important behavior.

## Bonus Features
You can choose to implement 1-2 features from this that you like:

1. Use relative time for the article's published times, e.g. 3 min ago, Yesterday 2 PM.
   - Choose appropriate relative-time boundaries and keep values current while the page remains open.
2. Give an option to the user to mark a news source as favourite.
   - If a favourite news source appears in search list, it should show before the news from other sources
3. If user has visited the main article for a news item from the "Read more" link, it should show "Visited" tag for such news items

Make sure you implement all the features in the main problem statement. Prioritize the work and document any items you
were not able to complete, along with the UX and architecture decisions you made.

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
