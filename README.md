# Storage and Visualization of Graph Data Using a Discography as an Example

A discography comprises all sound recordings released by a musician and provides an overview of the artist’s complete body of work. In most cases, discographies are presented as plain text or tables on various websites.

To demonstrate the scope and complexity of discography data, this project analyzes the discography of the well-known jazz musician Miles Davis. It consists of 307 tracks, 51 albums, 198 musicians, and 48 musical instruments, resulting in a total of 604 objects. All of this information is publicly available on websites such as Discogs (https://www.discogs.com) and Wikipedia (https://en.wikipedia.org).

Despite the richness of the data, it is typically presented in textual form only, making exploration tedious and unintuitive. The goal of this project is to develop a web application that visualizes complex discographies using minimal text and rich visual representations. The application is designed to make discography exploration intuitive and user-friendly and to support multiple datasets.

---

## Application Installation

According to the project requirements, the web application is implemented as a static application. For this reason, data storage is handled using JSON files. The results show that this approach is suitable for a successful implementation. A disadvantage of this solution is the increased effort required to manage and maintain datasets due to the high number of relationships between entities.

To visualize your own discography, follow these steps:

1. Clone the project from the GitHub repository:
   ```
   git clone git@github.com:prozb/miles-davis-project.git
   ```

2. Navigate to the project directory and install all required dependencies:
   ```
   cd miles-davis-project && npm install
   ```

3. Create four JSON files representing your discography using the required format.

4. Create a directory and move your discography files into this directory.

5. Move the directory containing your discography into the `public/discogs` directory so that the application can access it.

6. Start the application:
   ```
   npm start
   ```

7. Open your browser and navigate to:
   ```
   http://localhost:3000
   ```

---

## Discography Data Structure

Discographies must be created using the predefined JSON structure. If anything is unclear, refer to the example discographies of Miles Davis or Cream, which are located in the `public/discogs` directory.

| Musician JSON Object | Album JSON Object |
|---------------------|-------------------|
| ![Musician Object](https://github.com/prozb/miles-davis-project/blob/master/img/musician-json.png?raw=true) | ![Album Object](https://github.com/prozb/miles-davis-project/blob/master/img/album-json.png?raw=true) |

| Instrument JSON Object | Track JSON Object |
|-----------------------|------------------|
| ![Instrument Object](https://github.com/prozb/miles-davis-project/blob/master/img/instrument-json.png?raw=true) | ![Track Object](https://github.com/prozb/miles-davis-project/blob/master/img/track-json.png?raw=true) |

---

## Screenshots

![Album screen](https://github.com/prozb/miles-davis-project/blob/master/img/album-screen-nonav.png?raw=true)
![Instrument screen](https://github.com/prozb/miles-davis-project/blob/master/img/instrument-end-screen.png?raw=true)
![Musician screen](https://github.com/prozb/miles-davis-project/blob/master/img/musician-end-screen.png?raw=true)
![Track screen](https://github.com/prozb/miles-davis-project/blob/master/img/track-end-screen.png?raw=true)
![Search screen](https://github.com/prozb/miles-davis-project/blob/master/img/search-filter.png?raw=true)
![Tooltip](https://github.com/prozb/miles-davis-project/blob/master/img/tooltip-end-screen.png?raw=true)
![Special screen](https://github.com/prozb/miles-davis-project/blob/master/img/special-end-screen.png?raw=true)

---

## Technology Stack

- npm  
- React.js  
- JavaScript, HTML & CSS  
- reactstrap  
- material-ui  
- fortawesome  
- react-tippy  
- cytoscape-popper  
- react-router-dom  
- react-avatar  
