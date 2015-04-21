
# Mike's GitHub notes 
## Learning GitHub & Markdown 

:beer:
:walk:

**Resources I'm using**
- MacDown edit is the best that I found http://macdown.uranusjr.com/ I also considered
  - http://stackedit.io but it required internet access and http://25.io/mou/ but it's interface wasn't clean enough for me. 
- https://dabuttonfactory.com/ to make cute, easy buttons.
- [ReadWrite tutorial for GitHub](http://readwrite.com/2013/10/02/github-for-beginners-part-2) 
- [Write with Markdown on Google Drive](https://www.youtube.com/watch?v=VAx_Xf0KNfg)
- [SatckEdit on GitHub](https://github.com/benweet/stackedit)
- [Markdown cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet),  [Markdown basics](https://help.github.com/articles/markdown-basics/) and [GitHub Flavored Markdown (GFM)](https://help.github.com/articles/github-flavored-markdown/)
- [GitHub code school](https://try.github.io/levels/1) 
- we made iOS based on https://developers.facebook.com/docs/ios?locale=es_ES
- reference scheme url https://developers.facebook.com/docs/ios/getting-started?locale=es_ES
- learn iOS xcode https://www.youtube.com/watch?v=ZqKbN_C4Yvg
- download videos http://rg3.github.io/youtube-dl/download.html
- use `screen` to download without interruption http://stackoverflow.com/questions/11807688/how-to-detach-a-process-from-terminal-in-unix
- temporary email https://mailinator.com/



----------

###git commands
  - git status
  - git add -A
  - git commit -m "blurb about the changes"
  - git push
  - git pull
  - git checkout [branch name]   <-- this is the command for switching branches in Unix

----------------


Let's use this!
https://github.com/showcases/projects-with-great-wikis


**Mike took 'data objects' from Automatic. What do Fitbit, Jawbone, & Nest say? let's benchmark with them. Keep it simple.**

  - Specify read-only. Jawbone & Fitbit are read & write.
  - Specify JSON response only. Fitbit does JSON & XML.
  - 

**Jawbone** 

  - [pull data](https://jawbone.com/up/developer/structure) contains data (common objects & collections) and metadata (info related to the request itself)
  - [push notifications](https://jawbone.com/up/developer/pubsub) are "pub sub"
    - **Berman**, is there a different between a "callback" and a "push event"? 
  - [jawbone oauth diagram](https://jawbone.com/up/developer/authentication)
  - Adi votes for this convention

**Fitbit**

  - [pull Resources](https://wiki.fitbit.com/display/API/Fitbit+Resource+Access+API)
  - [push Subscriptions](https://wiki.fitbit.com/display/API/Fitbit+Subscriptions+API) "**subscribe** to any changes in a user's data." "notify via an HTTP callback"
  - [fitbit oath diagram](https://wiki.fitbit.com/display/API/OAuth+Authentication+in+the+Fitbit+API#OAuthAuthenticationintheFitbitAPI-TheOAuthFlow)

**Stripe**  
  - They use **objects**. Maybe we could say 'complex object' vs. notification. or just say that notifications are a type of object that you subscribe to vs. other objects that you request.
  - Among the objects is the **[event object](https://stripe.com/docs/api#event_types)**  
  - They have `data` as an `array` https://stripe.com/docs/api#pagination
 
 
 **Misfit**  
  - FAQ http://misfit.com/support
  - 


**Nest**

  - [subscriptions](https://developer.nest.com/documentation/cloud/nest-api-intro) that clients "listen" to for event changes
  - they don't seem to have the ability to pull datasets   
  - [Nest's oauth diagram](https://developer.nest.com/documentation/cloud/authorization-overview)

**Automatic**  
  - docs: https://www.automatic.com/developer/documentation/  



---------


## GET /users/profile/call TEMPLATE

DESCRIPTION OF THE CALL

### Resource URI

**`https://wapi.theneura.com/v1/users/profile/call`**

### Request query parameters

#### Required request parameters
- `required_parameter`:  description

#### Optional request parameters
- `optional_parameter`: description

### Request headers

#### Required request headers

- `authorization`: Bearer authorization token

#### Optional request headers

- `Cache-Control`: Specifies if the server should circumvent the server cache

## Response for `call` 

parameters returned & descriptions


### Example `call` request

```http
GET https://wapi.theneura.com/v1/users/profile/call
Authorization: Bearer asdf1234**************************
Cache-Control: no-cache
```

### Example `call` response

#### Headers
```http
status: 200 OK
version: HTTP/1.1
Content-Type: application/json
```
#### Body
```json
{
   }
```
 



