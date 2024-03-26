     **This Document for All backend API's**
     
##  **Home Page**

-    **URL**: <https://alike.io/>.
-    **API**: `homepage_stories_products`
    -  This Graphql used for **Handcrafted Holiday Packages** section.
      -  ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/004f3825-6818-4189-9c37-40309ff6f235)
      - **Query**:
           ```graphql
        query homepage_stories_products($pageSize: Int) {
        homepage_stories_products(pageSize: $pageSize) {
    items { 
      uid
      id
      url_key
      product_likes
      ins_days
      name
      short_description_alike
      ins_tags
      ins_city
      is_liked
      insider_data {
        insider_name
        insider_logo
        insider_id
        profile_url
        is_followed
        username
        __typename
      }
      ins_traveller_type
      image {
        url
        __typename
      }
      icons {
        icon_url
        label
        count
        __typename
      }
      sku
      type_id
      price_range {
        minimum_price {
          regular_price {
            value
            currency
            __typename
          }
          __typename
        }
        __typename
      }
      dynamicAttributes(fields: ["ins_city", "ins_tags"])
      __typename
    }
    __typename
     }
     }
     ```
           
   - **variables:**
        ``` graphql
              {
                 "pageSize": 9
              }
        ```

  - **API:** `currency`
    - This GraphQl is used for **currency**.
    - here are five types of currency code available `GBP`, `EUR`, `INR`, `USD`, `AED`.
    - ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/02b1109d-1dcf-44a3-b7fe-00ec5d0656e4)
    - **Query:**
        -  ```graphql
          {
           currency {
            ip_currency
            available_currency_codes
            base_currency_code
            base_currency_symbol
            default_display_currecy_code
            default_display_currecy_symbol
            default_display_currency_code
            default_display_currency_symbol
             exchange_rates {s
             currency_to
              rate
              __typename
                }
            __typename
              }
          }
           ```
  - **API:** `new_products`
    - this Graphql used for **Best Selling Experiences** section.
    - ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/2ad1088a-b293-447b-bf7d-8f1f37701048)
    - **Query:**
        ```graphql
            query new_products($input: NewProductsLimit!) {
           new_products(input: $input) {
            url_key
            id
            name
            __typename
            image {
              url
              __typename
            }        
            small_image {
              url
              __typename
            }
            thumbnail {
              url
              __typename
            }
            tour_cities
            tour_category
            exp_duration
            exp_good_for
            exp_languages
            exp_transport_available
            exp_ticket_confirmation
            exp_type_of_ticket
            exp_cancellation
            exp_included_in_touristor
            short_description_alike
            strike_price_value
            price_range {
               maximum_price {
                final_price {
                  value
                  __typename
                }
                __typename
              }
              minimum_price {
                final_price {
                  value
                  __typename
                }
                __typename
              }
              __typename
            }
            dynamicAttributes(fields: ["tour_cities", "tour_category"])
          }
        }
        ```
    - **variables:**
       - ```graphql
             {
                "input": {
                 "limit": 9
                }
             } 
          ```
    - **API:** `cart`
    - Cart GraphQl and Currency GraphQl default set for all pages.
    - ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/316ced0b-c97b-48eb-9a0b-158c2edee01a)
    - **Query:**
     - **variables:**
       ```graphql
           {
             "cart_id": "o7WaADKQ6ICyNefpLatbPgMZBqC013hZ"
           }
       ```


           
