     **This Document for All backend API's**
     
##  **Home Page**

-    **URL**: <https://alike.io/>.
-    **API**: `homepage_stories_products`
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
            ```
               {
                   "pageSize": 9
                }
                ```
   -  This Graphql used for **Handcrafted Holiday Packages** section.
   -  ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/004f3825-6818-4189-9c37-40309ff6f235)

  - **API:** `currency`
    - This GraphQl is used for `currency`.
    - here are five types of currency code available `GBP`, `EUR`, `INR`, `USD`, `AED`.
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
    - ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/02b1109d-1dcf-44a3-b7fe-00ec5d0656e4)
  - **API:** `new_products`
    - this Graphql used for `Best Selling Experiences` section.
    - 
           
