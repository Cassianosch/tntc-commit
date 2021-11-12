## Commits Specifications in the Project Structure

In this document we will cover the specifications and rules for commits that must be followed in projects.

### Summary

[Watch the video]()
Senha: tntc

We will be basing this on the commit convention specification that provides us with several simple rules for creating and explaining the commit history, which makes it easier and more automated. These specifications will be based on [CM](https://www.conventionalcommits.org/en/v1.0.0/#specification), but with some changes to the rules to fit the profile of the company. <br />

### The commit messages should be structured as follows:
> type[module/scope(optional)]: description
>
> [body(optional)]
>
>[footer(optional)]

##### Commits contain structural elements(types), to communicate what is being done within it.
1. **fix**           - Will correct an error in the code
2. **feat**          - Will add a new feature to the code
3. **refactor**      - Refactoring some part of the code, not adding a new feature or fixing a bug
3.1. **refactor!**   - breaking change (! is for attention)
4. **revert**        - Will reverse some part of the code/commit
5. **Finish v0.0.1** - Created a commit release
6. **style**         - For css, formatting, missing semicolons, syntax adjustment
7. **test**          - Add Test 
8. **perf**          - Add or adjusting code that improves the app's performance
9. **ci**            - Deployment Process
10. **chore**        - Process of building or adding tools related to this
11. **docs**         - Documentation Changes

#### Examples

>Input that a monetary value should be entered, went into production without the mask, but it was noted that it was **better has the masks**.

`feat[shopping-cart]: Added masking to the purchase value input` <br />
`feat: Added masking to the purchase value input`

---

>Had a bug in the input that a monetary value must be entered and went into production without the mask, **but should have gone with the mask**.

`fix[shopping-cart]: Added masking to the purchase value input`

---

>I thought of a way to improve the format of the for, and this will make the user list perform better

`perf[user]: list of all users`<br />
`With a reformulation in the code that performs the user loop, a better way to perform it was thought of, removing the comparison from the Name element`

---
---

>Removing support for node < 6

`refactor!: drop support for Node 6`<br />

---
> By default using [Smart Git](https://www.syntevo.com/smartgit/)




