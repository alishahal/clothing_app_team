# Item -< Purchases >- User

# User Stories: 
    * User will be able to browse clothing store for clothing
    * User can purchase item(s) of clothing

# MVP:
    * Should be able to see available clothing items
    * User should have cart with total items and total ticket
    * Clothing store should update stock if user selects a piece 
    
# Stretch Goals:
    * User can search clothing items by color
    * User can search by size
    * User can search by price
    * User can enter a discount code at purchase
    * Build more models once base is working
    ** Multiple purchases through multiple users 
    ** User Login 
    *** User can return and item of clothing
    

# Clothing Item Properties: (has a purchase, has a user through a purchase)
    * name
    * cost
    ** size
    ** stock
    
<!-- # Purhcase(Cart) (belongs to store and user)
    * has user/item id([4, 5, 6])
    * contains items from store belong to user
    * total items
    * total cost -->

# Purchase (belongs to store and user)
    * has user/store id 
    * contains items from store belong to user

# User Properties: (has many purchases, has many clothing items through purchases)
    * username  

<!-- # Clothing Properties: (belongs to store and user)
    * brand name
    * item category
    * item name
    * item size
    * item price -->

Stretch method example:

        # available_items = selected_item.tickets.where({ passenger_id: nil })

        # ticket_options = available_tickets.map do | ticket |
        #     {
        #         name: "#{ticket.number}: #{ticket.departure_city}-#{ticket.destination_city} ($#{ticket.price})",
        #         value: ticket
        #     }
        # end

        # ^^ Use line 52-59 when we add stock to items
