// index.js
import React, { useState } from "react";
import ReactDOM from "react-dom/client";
import "./index.css";
import { pizzaData } from "./data.js";
import "bootstrap/dist/css/bootstrap.min.css";

// Logo URL (replace with your own)
const logoURL = "https://image.similarpng.com/very-thumbnail/2020/05/Pizza-logo-design-template-Vector-PNG.png"; // Temporary logo link

function Navbar() {
  return (
    <nav className="navbar navbar-expand-lg navbar-dark bg-dark">
      <a className="navbar-brand d-flex align-items-center" href="#">
        <img src={logoURL} alt="Logo" width="40" className="mr-2" />
        Andy's Pizza Co.
      </a>
      <div className="navbar-nav ml-auto">
        <a className="nav-item nav-link" href="#home">Home</a>
        <a className="nav-item nav-link" href="#menu">Menu</a>
        <a className="nav-item nav-link" href="#aboutus">About Us</a>
        <a className="nav-item nav-link" href="#contact">Contact</a>
      </div>
    </nav>
  );
}

function Header({ isOpen }) {
  return (
    <header className="text-center py-4 bg-warning">
      <h1 style={{ fontSize: "48px", textTransform: "uppercase" }}>Andy's Pizza Co.</h1>
      {isOpen && <p className="mt-2">Authentic Italian Cuisine</p>}
    </header>
  );
}

function Pizza({ pizza, onToggleFavorite }) {
  return (
    <div className="pizza-item card m-2" style={{ width: "18rem" }}>
      <img src={pizza.photoName} alt={pizza.name} className="card-img-top" />
      <div className="card-body">
        <h3 className="card-title">{pizza.name}</h3>
        <p className="card-text">{pizza.ingredients}</p>
        <p className="card-text">${pizza.price}</p>
        {pizza.soldOut && <p className="text-danger">Sold Out</p>}
        <button
          className="btn btn-outline-danger"
          onClick={() => onToggleFavorite(pizza.name)}
        >
          {pizza.isFavorite ? "♥" : "♡"} Favorite
        </button>
      </div>
    </div>
  );
}

function Menu({ pizzas, onToggleFavorite }) {
  return (
    <div id="menu" className="menu text-center">
      <h2 className="my-4">Our Menu</h2>
      <div className="d-flex flex-wrap justify-content-center">
        {pizzas.map((pizza, index) => (
          <Pizza key={index} pizza={pizza} onToggleFavorite={onToggleFavorite} />
        ))}
      </div>
    </div>
  );
}

function Footer({ isOpen }) {
  const message = isOpen ? "We're currently open" : "Sorry, we're closed";

  return (
    <footer className="bg-dark text-white text-center py-3">
      <p>{message}</p>
      {isOpen && (
        <div className="text-center mt-3">
          <button className="btn btn-primary">Order Now</button>
        </div>
      )}
    </footer>
  );
}

function App() {
  const [pizzas, setPizzas] = useState(pizzaData);
  const [searchQuery, setSearchQuery] = useState("");
  const [showFavorites, setShowFavorites] = useState(false);

  const currentHour = new Date().getHours();
  const isOpen = currentHour >= 10 && currentHour < 22;

  const handleToggleFavorite = (pizzaName) => {
    setPizzas((prevPizzas) =>
      prevPizzas.map((pizza) =>
        pizza.name === pizzaName
          ? { ...pizza, isFavorite: !pizza.isFavorite }
          : pizza
      )
    );
  };

  const filteredPizzas = pizzas.filter((pizza) => {
    const matchesSearch =
      pizza.name.toLowerCase().includes(searchQuery.toLowerCase()) ||
      pizza.ingredients.toLowerCase().includes(searchQuery.toLowerCase());
    const matchesFavorite = showFavorites ? pizza.isFavorite : true;
    return matchesSearch && matchesFavorite;
  });

  return (
    <div className="container">
      <Navbar />
      <Header isOpen={isOpen} />

      <div className="text-center my-4">
        <input
          type="text"
          placeholder="Search pizzas..."
          value={searchQuery}
          onChange={(e) => setSearchQuery(e.target.value)}
          className="form-control w-50 mx-auto"
        />
        <button
          className="btn btn-secondary mt-2"
          onClick={() => setShowFavorites(!showFavorites)}
        >
          {showFavorites ? "Show All" : "Show Favorites"}
        </button>
      </div>

      <Menu pizzas={filteredPizzas} onToggleFavorite={handleToggleFavorite} />
      <Footer isOpen={isOpen} />
    </div>
  );
}

const root = ReactDOM.createRoot(document.getElementById("root"));
root.render(<App />);
