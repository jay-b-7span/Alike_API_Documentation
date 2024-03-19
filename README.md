     **This Document for Backend(GraphQl) customization **
     
##  **Insider Community**

-    The insider community is shown on home page of <https://alike.io/>.
-   **Module**: `Nik_InsiderPageGraphQl`
-   **Resolver**: `Nik\InsiderPageGraphQl\Model\Resolver\InsiderCommunity`
-   In the resolver file return data like id, name,profile_picture etc
    using insiderId.
-   **Admin Menu**: `STORE`->`Configuration`->`CUSTOM`-\>`Insider`-\>`Home Page Configuration`
     set the Insider Community text field. here admin set a coma
     separating **insider's ID** and showed it in insider community.

##  **Explore Cities Nearby**
-   Explore Cities Nearby is shown on <https://alike.io/cities/> page.
-   **Module**: `Nik_Cities`
-   Here `CategoryInterface` in Citycustom query for this block.
-   **Resolver**: `Nik\Cities\Model\Resolver\CityCustom`
-   **Admin Menu**: `Catalog`-\>`Category`-\>`Content`-\>`Explore
     Nearby` Here admin set a coma separated **city's ID** and showed it in
     Explore Cities Nearby.
-   In the resolver file return data name, image, and highlights load by
     Explore Nearby cities id.
