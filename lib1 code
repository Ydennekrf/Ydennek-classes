class Media{
  constructor(title) {
    this._title = title;
    this._isCheckedOut = false;
    this._ratings = [];
    
  }

  get title() {
    return this._title;
  }
  get isCheckedOut() {
    return this._isCheckedOut;
  }
  get ratings() {
    return this._ratings;
  }
  set isCheckedOut(value) {
    this._isCheckedOut = value;
  }

  checkOutToggle() {
    this._isCheckedOut = !this._isCheckedOut;
  }
  getAverageRating() {
    let ratingSum = this.ratings.reduce((ratingSum, ratings) => ratingSum + ratings, 0);
      return ratingSum / this.ratings.length;
  }
  addRating(value) {
    this.ratings.push(value);
  }
}

class book extends Media{
  constructor(title, author, pages) {
    super(title)
    this._author = author;
    this._pages = pages;
  }

  get author() {
    return this._author;
  }
  get pages() {
    return this._pages;
  }
}

class movie extends Media{
  constructor(title, director, runTime) {
    super(title)
    this._director = director;
    this._runTime = runTime;
  }

  get director() {
    return this._author;
  }
  get runTime() {
    return this._runTime;
  }

}

class CD extends Media {
  constructor(title, artist, songs) {
    super(title)
    this._artist = artist;
    this._songs = songs; 
  }
  get artist() {
    return this._artist;
  }
  get songs() {
    return this._songs
  }
}

const historyOfEverything = new book('a short history of everything', 'Bill Bryson', 544)
const starWars4 = new movie('StarWars: A New Hope', 'George Lucas', '121 min')
const starWars5 = new movie('Star Wars: The Empire Strikes Back', 'George Lucas', '124 min')
const fellowshipOfTheRing = new book('Lord of the Rings: The Fellowship of the Rings', 'J.R.R. Tolkien', 423)
const ledZepplin1 = new CD('1', 'Led Zepplin', '1. Good Times Bad Times// 2. Babe Im Gonna Leave You// 3. You Shook Me// 4. Dazed and Confused// 5. Your Time is Gonna Come// 6. Black Mountain Side// 7. Communication Breakdown// 8. I Cant Quit You Baby// 9. How Many More Times')

historyOfEverything.checkOutToggle();
console.log(historyOfEverything.isCheckedOut);
historyOfEverything.addRating(4);
historyOfEverything.addRating(5);
historyOfEverything.addRating(4);
console.log(historyOfEverything.getAverageRating());
console.log(starWars4.)
