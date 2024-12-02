# CustomCADs Pages

- Public (accessible to all) pages:
  - Error pages (404, 401, 403, 502)
  - Info pages (Roles, Printer, Privacy Policy)
  - About us page (including an offer to join the dev/designer teams by emailing us at customcads@gmail.com)
  - Gallery page (including searchbar with filter and sort options, grid/list option for products, and pagination - products show only the image)
  - Product page (details of the items in Gallery page, full Product info, visualized Cad, Tweak and Add to Cart buttons (disabled if not a Client))

- Guest (only without account) pages:
  - Home page (including quick info cards and useful shortcuts)
  - Login page (username and password fields, should have a link to Register page)
  - Register page (username, email, password, confirm password fields + optional first and last name, should pick between Client and Contributor registration, should have a link to Login page)
  
- Client (registered as client) pages:
  - Dashboard page (useful widgets, like recent orders and total count of orders grouped by status, closable info about File vs Delivery)
  - Cart page (the Client can review the Items he's added to his Cart, and can Purchase them all at once.)
  - Purchase page (after cicking on Cart page's Purchase button, Credit Card info should be requested here and the transaction should be processed, and depending on what the Client chose he'll either receive the 3D File, or trigger a Delivery, or both)
  - Order Form page (the Client can describe in detail what he wants, then order it)
  - Orders page (contains all the Client's Оrders, and summarized info about them, includes a searchbar with filter and sort options)
  - Order page (when an order from Orders page is clicked, it leads the Client here, and he can view the order details and, depending on status, edit as well (straightforward if Pending, needs to be a requset if Accepted or Begun, forbidden if Finished))
  - Carts page (contains all the Client's Carts and info summarized about them, includes a searchbar with filter and sort options)
  - Cart page (when a cart from Carts page is clicked, it leads the Client here, and he can view the full Cart info and all its Items, includes a searchbar with filter and sort options)
  - Item page (when an item from Cart page is clicked, it leads the Client here, and he can view the full Item info, includes a searchbar with filter and sort options)
  - Cads page (contains all the Client's Cads - completed Orders and Cart purchases go here if 'As a File' option is chosen)
  - Cad page (when a cad from Cads page is clicked, it leads the Client here, and he gets to visualize and tweak his Cad, and also Download it)
  - Deliveries page (contains all the Client's Deliveries - completed Orders and Cart purchases go here if 'As a Delivery' option is chosen)
  - Delivery page (when a delivery from Deliveries page is clicked, it leads the Client here, and he gets to see the full info of his Delivery, and also Cancel it)
  
- Contributor (registered as contributor) pages:
  - Dashboard page (useful widgets, like recent products and total count of products grouped by status, closable info about Upload vs Sale)
  - Upload page (the Contributor can provide Product info here and upload it to the Gallery (though it must be verified by a Designer first))
  - Sell page (the Contributor has chosen a product to sell and was brought here, to negotiate a price and)
  - Products page (contains all the Contributor's products, includes a searchbar with filter and sort options, with Sell All shortcut option, seperation between Contributor's Products, Products for Sale, and Sold Products)
  - Product page (when a product from Products page is clicked, it leads the Contributor here, and he can view the product details and edit as well, includes a Sell button)

- Designer (hired as designer) pages:
  - Dashboard page (useful widgets, like recent accepted orders and checked products, closable info about Order Completion and Product Verification)
  - For Sale page (the Designer can choose from Contributors' For Sale products and buy the ownereship rights to them, has a Buy button)
  - Buy page (after cicking on For Sale page's Buy button, Credit Card info should be requested here and the transaction should be processed, with the Product being removed from the Contributor's page and added to the Designer's)
  - Upload page (same as Contributor's Upload page, except that it goes straight to the Gallery)
  - Products page (same as Contributor's Products page, except that no Sell functionality or distinction is provided)
  - Product page (same as Contributor's Product page, excepte that no Sell functionality is provided)
  - Client Orders page (used for answering Clients' Orders, seperations between all Pending orders, the Designer's Accepted orders, the Designer's Begun orders and the Designer's Finished orders (with the last one having the option to hide an order, and a Hidden subsection))
  - Contributors Products page (used for validating Contributors' Products, seperation between Unchecked products, the Designer's Validated products and the Designer's Reported products)

- Administrator (working as higher-ups) pages/panel:
  - Tables 
    - All Users table, including info like Id, Role, Username, Email, Account Verified, First and Last name, etc., including a searchbar with filter and sort options
    - All Roles table, including info like Id, Name, Description, and Users Count
    - All Orders table, including info like Id, BuyerName, Name, Description, Order Date, Status, DesignerName (nullable)
    - All Products table, including info like Id, CreatorName, Name, Description, Upload Date, Status, Cost, Purchased Count
    - All Categories table, including info like Id, Name, Products Count
    - All Deliveries table, including info like Id, Delivery Status, Address, Type (custom or item), and Linked Order
  - CRUD
    - Able to create, update and delete Categories.
    - Able to create, update and delete Roles.
    - Able to create, update, delete User Accounts. Can ban any User, usually a reported one.
    - Able to create, update and delete Products. Can ban any Product, usually a reported one.
    - Able to create, update and delete Orders. Can ban any Order, usually a reported one.
