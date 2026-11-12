# Movie Rating Classification

> **DSA 495 Topic Brief**
>
> Replace the bracketed prompts below with your team’s information. Keep this file at the root of your team’s project repository and name it `README.md`.

## Before You Begin

- Create **one shared project repository per team** and continue using it through the end of the semester. Do not create separate repositories for the Topic Brief and later stages of the project.
- The repository name must begin with the case-sensitive prefix **`DSA495`**, such as `DSA495-news-classification`. After the prefix, feel free to choose a creative and distinctive team name; it does not have to describe your task or topic. A repository whose name does not begin with `DSA495` will receive zero credit for the Topic Brief.
- Complete every required section and item below. Anything labeled optional may be left undecided! If another required item does not apply, write “Not applicable” and briefly explain why. Feel free to add sections as needed, but keep the brief concise.
- Make sure the repository is accessible to the instructor by choosing one of the following options:
  1. **Public repository:** No collaborator invitation is required.
  2. **Private repository:** Add the instructor as a collaborator using the GitHub username `SerenaYKim`.
- Do not upload sensitive or restricted information to GitHub, even in a private repository. If your project uses such data, keep it in a shared team drive and use GitHub for code, documentation, and other materials that can be shared safely.

## Team Members

- Lucas Hopey
- Caleb Cockerham

## One-Sentence Task

**Given [the text or other input], we will [analyze, classify, retrieve, compare, or generate] [the intended output].**

Given the movie review comment, we will classify the predicted rating of that movie based on the review and whether or not it will be classified as fresh or rotten. 

## Illustrative Input and Desired Output

- **Example input:** "It's a horrific mish-mash of other films that ends with two CGI monsters punching each other into walls while screaming about “ultimate power”." 
- **Desired output:** Rotten

## Background and Starting Point

People are very passionate about movie ratings so trying to build a model that can accurately predict how a person will review a movie based on their description of their rating is very helpful when trying to differentiate a positive from a negative review just based on the words alone. 

## Intended Output and Success

The intention of this project is to analyze movie rating comments to predict labels of the movie review fresh/rotten. These are the labels commonly used by ratings sites and theatres to determine the public opinion of the movie. People who would use this output are studios who want to learn how a movie was received based on text comments.

**Success statement:**
Sucess for this project would look like a model that can effectively predict the score given by a particular user based on the text they included in that review. 

## Preferred Data

### Corpus

The collection of text is a collection of movie rating comments. One observation in this data set represents a review. There are no other useful fields as it is just the review and the fresh/rotten determinant field. The corpus is approximately 480 thousand movie rating comments with 2 fields.

### Source and Access

- **Dataset or corpus name:** Rotten Tomatoes Reviews
- **Original source organization or creator:** Ulrik Thyge Pedersen 
- **Original collection process:** Data was gathered by the creator and sourced from Rotten Tomatoes.
- **Direct link:** https://www.kaggle.com/datasets/ulrikthygepedersen/rotten-tomatoes-reviews
- **Access method:** Download (CSV file)
- **Access, licensing, privacy, or redistribution considerations:** None identified
- **Backup corpus (optional):** Not needed at this stage

### Examples

Within each rotten tomato review we have the text of the review. We also are given the freshness given by the reviewer.

**Review:** It would be difficult to imagine material more wrong for Spade than Lost & Found.
**Freshness:** Rotten

**Review:** Slight, contained, but ineffably soulful.
**Freshness:** Fresh

**Review:** Everyone in "The Comedian" deserves a better movie than "The Comedian."
**Freshness:** Rotten

### Fit with the Task

We are given the review text and whether or not it is classified as fresh or rotten which will allow us to train the model and then test its prediction accuracy against held out observations.

## Feasibility and Immediate Next Steps

- **Minimum viable project:** Using a small subset of the larger overall data and perform text analysis to predict fresh or rotten reviews.
- **Data-access check:** The data has been downloaded and viewed.
- **Largest current risk:** The largest risk is deciphering the sentiment from movies in general when not factoring in the type of movie as being scared in a horror movie is different than being scared in a romance movie.
- **Backup plan:** The scope could be narrowed down to one category of movies. For example, just analyzing action movies.
- **Next two actions:**
  1. Determine modeling techniques and begin framework — Lucas and Caleb — October 30
  2. Finalizing modeling and evaluate predictions — Lucas and Caleb — November 6

## Possible Text-Analysis Method and Evaluation (Optional)

Not yet decided.

## Questions for the Instructor

- What methods and evaluation techniques would you suggest for this project idea?
- How would you address concerns about computing power given the data set is so large?
- No additional questions at this time.

## AI-Use Statement

**Documentation and Idea Generation**

No AI was used for the idea of this project, the gathering of the data, or the completion of this README.md file.

**Coding**

Gemini AI in Google Colab was used for the data cleaning, modeling, and evaluation to explain and resolve errors and validate proper coding techniques. The use of this AI helped our progress by understanding what our coding errors were and why they occurred. It also helped us improve our code by learning about new options in the functions, such as cmap in the ConfusionMatrix() function to add color.
