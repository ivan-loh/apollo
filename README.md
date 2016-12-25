# apollo

Custom content delivery server

- [ ] Basic Data Posting
- [ ] Access Control
- [ ] Content Serving
- [ ] Content Tracking
- [ ] Customized Content


## Application Structure

```
apollo
│
├── main.go
│
├── conf
│   └── app.conf
│
├── controllers
│   └── action.go
│   └── assets.go
│
└── tests
    └── default_test.go
```

                                                                                                           
## APIs                                                                                                      
                                                                                                              
### /action                                                                                                
                                                                                                              
**URL:** `http://apollo/action`

**METHOD:** `POST`


User behaviour logging, this is a general channel to log any user activity or action, the payload is context relevant to the action bit is optional, eg a user registration for a login base system should include user information where as a login action can be empty.

**Data Needed:**
- id
- mac
- name
- action
- payload
