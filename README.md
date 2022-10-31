# Weekend Challenge 11 - React-Redux Feedback Form

## Instructions

Reviewing code is an important role developers play. We're going to practice reviewing code from others.

- Get the repo url from your partner
- Get your partner's project running on your computer
- Review the code from your partner and give relevant feedback
- Complete the Markdown section and submit that in the notes section on the assignment app. (Make sure you include who's code you reviewed.)

Practicing compassionate code reviews is important (you can learn more from this video on the topic: https://www.youtube.com/watch?v=Ea8EiIPZvh0 )

## Review Checklist

## Base Required Features 

- Multi-Part Form:  
  - [ X ] Able to add feedback
    - [ X ] Data collected on individual pages & components
    - [ X ] Click on next takes you to the next page in sequence
    - [ X ] Data saves in DB after *all* the parts are completed (not piecemeal)
    - [ X ] Thank you page takes you back to the first view
    - [ X ] Old Data is cleared on form completion

- Client code:
  - [ X ]  Individual components for each form part
  - [ X ]  Redux setup complete
    - [ X ] Store linked to react with `<Provider>`
    - [ X ] Store setup with reducer(s) and logger middleware 
  - [ X ] Reducers & Actions Working
    - [ X ] Actions are in SCREAMING_SNAKE_CASE and semantically named
    - [ X ] Actions have a `type` key, and `payload` if sending data
    - [ X ] Reducers are returning a new state, or the old state (not mutating)
    - [ X ] Reducers are using spread correctly (to keep old data, while adding new)
  - [ X ] Review Component shows at all times with current redux state
  - [ X ] React-Redux Working
    - [ X ] Dispatching actions onClick
    - [ X ] Grabbing data from the redux store with `useSelector`
  - [ X ] Axios POST request to add feedback


- Server code:   
  - [ X ] Router made for GET, POST


## General Items
Feedback should be provided for these items, but they do not impact scoring.

- Git 
  - [ X ] Multiple git commits showing incremental progress
  - [ X ] Commits are descriptive of the changes made or feature added 
  - [ X ] Has .gitignore with node_modules
  - [ X ] Readme file updated (assuming this is previously discussed)
- Code Style 
  - [ X ] Appropriate amount of code comments
  - [ X ] Code is consistently formatted
- Client
  - [ X ] Appropriate use of HTML tags
  - [ X ] Basic CSS styling with margins/padding


## Stretch Goals
First must be complete for score of  _Exceeds Expectations_

- Previous Steps
  - [ ] allows a user to go to a previous step, either directly or by cycling backward thru the steps
  - [ X ] user can upate their score for a step
    - [ ] new score is validated to not be empty
    - [ X ] redux is updated with new score
  - [ X ] user can continue on to review page and submit as in Base Mode


- Admin View
  - [ X ] All entries are visible with correct data from inputs
    - [ X ] Most recent is at the top
  - [ X ] Can Delete an entry
    - [ X ] User is prompted before deleting
  - [ X ] Axios GET request to get all feedback for `/admin` view in componentDidMount

  Busywork Goals, consider removing or making more useful

- [ X ] Styling with Material UI
- [ X ] Ability to flag a feedback item on `/admin` for further review
- [ ] Deployed to Heroku


## Markdown

```
Hey _TORMOD__,

General Feedback.

---
| Functional Requirements | Complete? |
| --- | :---: |
| Multi page form with client side routing and navigation (next button) | no |
| Data stored in Redux when navigating from page to page | no |
| User is notified when trying to leave a blank score | no |
| Review Component displays scores and comments from current redux state | no |
| Submit button sends data to the server via Axios | no |
| Confirmaion Page displays after data is POSTed to the server | no |
| Button on Confirmation Page clears Redux and starts a new survey | no |
| Views are broken down into components | no |

---
### Notes:

Notes on the above Functional Requirements.

---
| General Items | Complete? |
| --- | :---: |
| More than 15 git commits | yes |
| Commits are descriptive of the changes made or feature added | at the start, yes, at the end, no |
| Readme file updated | yes |
| Appropriate amount of code comments | yes |
| Code is consistently formatted | yes |
| Server code organized with router & module files | yes |

---
### Notes:
Hey great job Tormod, I really like the added pictures, it made the vibe of the overall project much better. 

I also really liked your incorporation of MUI, especially the prompt box when the delete item button is clicked. You set this project up with a lot less code than I thought would be needed, so it's really cool to see you being efficient in that way!

I do have a few things I think could have been improved, respectfully.

1. It would have been nice to see a physical "back" button for each page, rather than just relying on clicking the browser's back button. For all intents and purposes, this works fine, but would have made the use interface easier to digest.

2. I also think ideally you'd want to start each component page with empty values, and incorporate a 'required' attribute. The way it's set up now, if there's a bunch of jokesters wanting to spam your database, they can just keep pressing next over and over and over again without any deterrent to slow down. 

3. Your flagged button works when you click it, unless it's clicked directly on the flag. It would be nicer to also see it centered in the button. It's not a huge deal but it was a little confusing when it wouldn't switch back for me at first.

4. Similar problem as before, if you click on the delete icon in the delete button, and confirm you'd like to delete the row, it will not delete it. 

5. Overall the project looks great and the way you coded it was super clever! Nice job.

Notes on General Items

```
