     **This Document for Backend(GraphQl) customization **
     
##  **Home Page**

-    **URL**: <https://alike.io/>.
-    **API**: `cmsPage`
      - **query**:
            - ```
                query cmsPage($identifier: String) {
                   cmsPage(identifier: $identifier) {
                   identifier
                   url_key
                   title
                   meta_title
                   meta_description
                   meta_keywords
                   __typename
                    }
                 }
               ```
