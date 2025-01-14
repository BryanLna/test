.header {
    background-color: gray;
    color: white;
    padding: 10px 20px;
    position: fixed;
    top: 0;
    left: 0;
    right: 0;
    z-index: 1000;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.logo {
    font-size: 30px;
    font-weight: bold;
}

.menu.desktop-menu {
    display: flex;
}

.menu-list {
    list-style: none;
    margin: 0;
    padding: 0;
    display: flex;
    gap: 20px;
}

.menu-list li a {
    text-decoration: none;
    color: white;
    font-size: 16px;
    font-weight: bold;
    transition: color 0.3s ease;
}

.menu-list li a:hover {
    color: yellow;
}

.burger-menu {
    display: none;
    flex-direction: column;
    cursor: pointer;
}

.burger-menu .line {
    background-color: white;
    height: 3px;
    width: 25px;
    margin: 4px 0;
    transition: background-color 0.3s ease;
}

.burger-menu.active .line {
    background-color: lightgray;
}

.menu.mobile-menu {
    display: none;
    position: fixed;
    top: 60px;
    left: 0;
    right: 0;
    background-color: gray;
    padding: 10px 20px;
    z-index: 999;
}

.menu.mobile-menu.active {
    display: flex;
    flex-direction: column;
    gap: 15px;
}

.menu.mobile-menu .menu-list {
    display: flex;
    flex-direction: column;
}

.menu.mobile-menu .menu-list li a {
    color: white;
    text-decoration: none;
    font-size: 20px;
}

@media (max-width: 768px) {
    .menu.desktop-menu {
        display: none;
    }

    .burger-menu {
        display: flex;
    }

    .menu.mobile-menu {
        display: none;
    }
}
