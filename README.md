# KPMG Legal Tech Developer Technical Assesement

## Introduction

The aim of this exercise is to assess your ability to write well defined HTML, CSS and JavaScript using the latest patterns and technologies in a mobile first approach. The brief is fairly open and there's no right or wrong way to approach this.


## Brief

1. As a user I'd like to be able to view the locations of the company plotted onto a map and then be able to tap/click on those points to see more detail about the company.

2. As a user I'd lke to be able to see the companies in a table and be able to filter on the fees and sector.

## Data

We've provided an endpoint that can be accessed using the following URL: [https://run.mocky.io/v3/7cb595ed-2882-4dc7-8179-d38d0b9c9d13](https://run.mocky.io/v3/7cb595ed-2882-4dc7-8179-d38d0b9c9d13)

You can also find a sample of the data: [companies.json](companies.json)

### Types

```js
/** The response type of the API call */
type Reponse = Company[];

/** Company Entity */
interface Company {
  id: number;
  company: string;
  sector: string;
  stockSymbol: string;
  address: string;
  location: Location;
  fees: Fees;
}

interface Fees {
  amount: string;
  currency: string;
}

interface Location {
  latitude: number;
  longitude: number;
}
```


## Technology

Since the purpose of this exercise is to assess your HTML, CSS and JavaScript abilities, you're welcome to frameworks like Bootstrap, React, Vue etc.

## The Deliverable

* A bundled/archived repository showing your commit history or a link to an accessible repository with your work in (Github offers free private repository hosting).

* A Readme.md file explaining the your pre-build plan and the decisions you made when solving this task, such as framework, UI/UX etc.
* A Build.md file giving any instructions required to run your solution