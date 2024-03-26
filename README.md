     **This Document for Backend(GraphQl) customization **
     
##  **Home Page**

-    **URL**: <https://alike.io/>.
-    **API**: `cmsPage`
      - **query**:
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
        ```graphql
               {
                   "pageSize": 9
                }
                ```
   -  This Graphql used for **Handcrafted Holiday Packages** section.
   -  ![image](https://github.com/jay-b-7span/Alike_API_Documentation/assets/114227263/004f3825-6818-4189-9c37-40309ff6f235)

