# **Rick and Morty Character Viewer**

The Rick and Morty Character Viewer is a React application that allows users to explore characters from the popular TV show "Rick and Morty." It utilizes the [Rick and Morty API](https://rickandmortyapi.com/documentation/#rest) to fetch character data and provides a user-friendly interface with pagination for easy navigation.

## ** Installation **

- Install project dependencies

```bash
npm install
```

- Start the development server

```bash
npm start
```

## **Features**

This project consists of several components, each serving a specific purpose:

### **Card.tsx**

The **Card.tsx** component is responsible for fetching and displaying character data. It includes the following functionalities:

- Utilizes the **useState** hook to manage character data, pagination information, and the current page.
- Uses the **useEffect** hook to fetch character data from the [Rick and Morty API](https://rickandmortyapi.com/documentation/#rest) based on the current page when the component mounts or when the **currentPage** changes.
- Provides functions to handle previous, next, and page click actions.
- Renders character cards with names and images.

### **Pagination.tsx**

The **Pagination.tsx** component is dedicated to rendering pagination controls. It includes the following features:

- Contains a function called **getPageNumbers** to calculate page numbers based on the current page and total pages.
- Renders "Previous" and "Next" buttons with appropriate click handlers and disabled states.
- Renders page number buttons with click handlers to allow users to jump to specific pages.

### **RickandmortyApi.tsx**

The **RickandmortyApi.tsx** file defines constants and interfaces related to the Rick and Morty API. It includes:

- BASE_URL: The base URL for the Rick and Morty API.
- Character interface: Describes the structure of character objects, including name and image properties.
- PageInfo interface: Defines the structure of pagination information, including count, pages, next, and prev properties.
- PaginProp interface: Specifies the structure of props used by the **Pagination** component.

### **Page.tsx**

The **Page.tsx** component serves as the main application page where the other components (**Card** and **Pagination**) are used to build the user interface.

## **Project Structure**

The project is organized as follows:

- Card.tsx: This React component handles character data fetching and display, as well as pagination.
- Pagination.tsx: Another React component that renders pagination controls.
- RickandmortyApi.tsx: Contains constants and interfaces related to the Rick and Morty API.
- page.tsx: The main application page where the components are assembled.
