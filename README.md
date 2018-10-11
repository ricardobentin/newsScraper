# newsScraper

newsScraper is an an application that allows users to scrape articles from the Wall Street Journal homepage and allows users to take notes on each story. Once a user has saved a note, they can update it later or choose to delete it.

If a user wants to scrape a new set of articles, they just need to hit the scrape articles button.

To use the application, go here: https://limitless-earth-96609.herokuapp.com/

Scraping technique description:

This app uses a combination of Axios and Cheerio to do the scraping of the Wall Street Journal. Each headline and link is saved in a MongoDB database inside of an Articles document. Once a user decides to make a note on an article. That note's title and body are saved inside of a Notes document but the Object Id of the note is also subsequently pushed into the Article document so as to create a relationship between the article and the note.

newsScraper Demo:

<img src="https://github.com/DevTinder/newsscraper/blob/master/public/img/demo.gif" alt="demo">

Packages used:
* Axios
* Body-Parser
* Cheerio
* Express
* Express-Handlebars
* Mongoose
* Morgan
* Request

Happy scraping!