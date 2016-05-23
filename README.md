Silhouette Seed Template Slick API REST
=====================================


## Fonctionnalités

* Sign Up
* Sign In (Credentials)
* Social Auth (Facebook, Google+, VK, Twitter, Xing, Yahoo)
* Two-factor authentication with Clef
* Dependency Injection with Guice
* Publishing Events
* Avatar service
* Remember me functionality
* [Security headers](https://www.playframework.com/documentation/2.4.x/SecurityHeaders)
* [CSRF Protection](https://www.playframework.com/documentation/2.4.x/ScalaCsrf)


##Utilisations

#Requête                          #Réponse
    GET /
                                        {
                                          "message": "api rest play slick silouette"
                                        }

    POST /signUp
    {
    "firstName":"abdou",                {
      "lastName":"fall",                           "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIyLUFCSGtYYVY4VTZRUjV1dityaVJsRHBkakpkd1wveGUzSmpWZVwvdU02YkNiU0pvM1ZYZVNtNG5FZ1JvS0dtS0ROK0pWdEhnd2VXUG1RVUF4cVJVb2dPZ2p1Q28xNjNLNCtOQ0dsQiIsImlzcyI6InBsYXktYW5ndWxhci1zaWxob3VldHRlIiwiZXhwIjoxNDYzNjk5MjI0LCJpYXQiOjE0NjM2NTYwMjQsImp0aSI6IjZmNmNiNzZmMWVlZjZmNzg3NTAyNmRhZWU4YTU5OWQzZmRkNTg5ZDRhM2NhNDVkMTI5MTk2YjczNzcyNGI3NjRiNmViMzI1ZWU4NGE2NDU0ZmZkMTYxZGFmYWEzYzhkNDQ0ODhkM2NhOTkwMDM3NjMxMjlmODM1NmVmMTk2NWIyODMyNjRhNmE1ZGJiOTNhY2NhZThkYTAwOGNlNTE2ZGMxNThiNTA4NDY4MGJmY2E3MDhhNTQxZGZkYmI2ODY4YWVmNDY4YTNiODcyY2NiMmM1NmMyYjJjZDhlYWRhMDBjNWVmY2E1NGU0NWM1NmIzMjRmNDA4ODA1YTgzYmZjMjkifQ.SxlBDqMSOgLjK8Ieahmom77IB8qhuuxzbWOA7TFDR9s"
      "email": "fall@gmail.com",        }
       "password": "abdoufall"
    }


    POST  /user
    HEADERS :
    X-Auth-Token : TOKEN                {
                                           "userID": "8d01c38b-6e4f-4777-8078-64a2e81f7cae",
                                           "loginInfo": {
                                             "providerID": "credentials",
                                             "providerKey": "fall@gmail.com"
                                           },
                                           "firstName": "abdou",
                                           "lastName": "fall",
                                           "fullName": "abdou fall",
                                           "email": "fall@gmail.com"
                                         }


    POST  /signIn
                                                  {
                                                    "token": "eyJ0eXAiOiJKV1QiLCJhbGciOiJIUzI1NiJ9.eyJzdWIiOiIyLVRORzFrN1FsWEw4XC9vRUFCN3dONVpWN2xzaEVEOU9LR2VPem1XdksxcGZyeVZkZ2xTcVFoQkRzdnd4NmM1akFOUU5oWm1td2FvaVZDN2x4OEJPb21TeFJSVDJ2WklNaUJyTlo5IiwiaXNzIjoicGxheS1hbmd1bGFyLXNpbGhvdWV0dGUiLCJleHAiOjE0NjYyNDg1MjksImlhdCI6MTQ2MzY1NjUyOSwianRpIjoiYjk2N2MyMWY4MGU0N2U1MTIyZmM3Yzc1M2M4OTE5ZGQzMmQ0NjQ3Njc3OTdkMzBkYjE2MDMwNzYwN2FlNTUyN2UxZWZhNDlkNGM3N2JjMzNkOTkxMDYxMWRlNGNkZjg5MGViNjhmZTVlNmE3OWEwMmZkZWJmMTBjZGI4Yjg2NjAzMjIwMmYzNjI3MmI1NWYwNTFhZGUyYTUzYjY3ZTk0NGI0MjhjOWYwYzIxNWIzYTIyYzI0MzUzYzY2MTUzYzJhYzUwMjMxYjQ0YjU5Y2RjZDVjZGQzYmMxOWI0ZTkyZGM1MjQwODBkOGIxMzlkZmQ3Y2I0YjhhMjA0MDZlNGY5YSJ9.zvtoGgxsLDwngagEZ2FYM4B-nOMzYy-6sCw0C8brblM"
                                                  }
       {
       "email": "fall@gmail.com",
        "password": "abdoufall",
         "rememberMe": true
        }


## Documentation

Consult the [Silhouette documentation](http://silhouette.mohiva.com/docs) for more information. If you need help with the integration of Silhouette into your project, don't hesitate and ask questions in our [mailing list](https://groups.google.com/forum/#!forum/play-silhouette) or on [Stack Overflow](http://stackoverflow.com/questions/tagged/playframework).


# License

The code is licensed under [Apache License v2.0](http://www.apache.org/licenses/LICENSE-2.0).
