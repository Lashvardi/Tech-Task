# 🌍 Angular Country Explorer - **Task**

> 🌐 Instructions are available in other languages: [Georgian](README.ge.md),

Welcome to your assignment! You are going to build a Country Explorer web application using Angular and the Restcountries API. Get ready to showcase your Angular skills!

## 🎯 Objective

Your mission is to create a dynamic web application that fetches and presents information about various countries using the Restcountries API. Furthermore, you are required to use an image API to fetch and display captivating images of each country.

## 📚 Table of Contents

- [Required Features](#-required-features)
- [APIs to Integrate](#-apis-to-integrate)
- [Design References](#-design-references)
- [Technologies to Use](#-technologies-to-use)
- [Code Implementation Hints](#-code-implementation-hints)
- [Installation & Setup](#-installation--setup)
- [Evaluation Criteria](#-evaluation-criteria)
- [Submission Guidelines](#-submission-guidelines)

## 💡 Required Features

Your application should be able to:

1. Display a list of all countries. Each country entry should at least include the country's name and flag.
2. Allow users to click on a country to view more detailed information - population, area, languages spoken, etc.
3. Provide a search function that enables users to search for a country by name.
4. Fetch and display a relevant image for each country using an Image API of your choice.

## 🌐 APIs to Integrate

- [Restcountries API](https://restcountries.com/): Fetch information about different countries.
- Your choice of Image API: Fetch and display images related to each country.

## 🎨 Design References

Feel free to take inspiration from the following resources for the design of your application. Remember, a good user interface enhances the user experience!

- [Live Preview](https://angular-country-app.vercel.app/)

## 🛠️ Technologies to Use

- Angular
- Restcountries API
- Your choice of Image API

## 💻 Code Implementation Hints

One of the main objectives of this task is to get hands-on experience with Angular's `HttpClient`. It will be used to handle all HTTP requests to your APIs. Make sure to import it in your app module:

```typescript
import { HttpClientModule } from '@angular/common/http';

@NgModule({
  ...
  imports: [
    ...
    HttpClientModule,
    ...
  ],
  ...
})
export class AppModule { }
```


```typescript
import { HttpClient } from '@angular/common/http';

@Injectable({
  providedIn: 'root',
})
export class DataService {
  constructor(private httpClient: HttpClient) { }
}
```


## 🔧 Installation & Setup

You are expected to:

1. Fork and clone this repository.
2. Navigate to your cloned repository.
3. Install Angular CLI if you haven't done so yet: `npm install -g @angular/cli`
4. Install the necessary dependencies: `npm install`
5. Start the application: `ng serve`
6. Open your browser and navigate to `http://localhost:4200`.

## 📋 Evaluation Criteria

Your task will be evaluated based on:

1. Functionality: Does the application work as expected?
2. Code Quality: Is the code clean, readable, and well-organized?
3. User Interface: Is the application easy to navigate and visually appealing?
4. Responsiveness: Does the application display correctly on all screen sizes?
5. Error Handling: How does the application handle potential errors, such as a failed API call?

## 📥 Submission Guidelines

Once you've completed the task, submit a link to your repository via the designated submission platform.

Best of luck, and have fun building your country explorer! 🚀
