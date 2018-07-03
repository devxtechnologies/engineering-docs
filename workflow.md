# Workflow

1. Plan item
2. Assign card
3. Create branch
4. Write code
5. Pull request and code review
6. Stakeholder review
7. Deploy

## Plan Item

Product manager creates Trello card.

## Assign Card

When an engineer needs a new item they have a card assigned by the product manager and discusses details.

## Create Branch

* `master` should always be ready for production and deployable.
* `master` should never be committed to directly.
* `develop` is the primary development branch.
* Create new working branches off of `develop` with prefixes based on the item
  type.

## Write Code

## Pull Request and Code Review

1. When an item is completed create a Github pull request (PR).
2. Have another engineer review and approve the PR.
3. After pull request is approved, merge to develop.
4. Deploy `develop` to development server.

## Stakeholder Review

Have the stakeholder review the implementation before deployment to production.

## Deploy

1. After stakeholder approves merge `develop` into `master`.
2. Update `changelog` and add `tag` for versioning. 
3. Deploy `master` to production server.
