This API is going to create a node person for exisiting user:
# The response you'll get in JSON:
```json
{
    "node": {
    "communication_type": null,
    "controlling_node_id": null,
    "facebook_user_id": null,
    "google_place_id": null,
    "google_user_id": null,
    "netbios_domain": null,
    "netbios_name": null,
    "netbios_role": null,
    "node_alias": null,
    "node_type": "person",
    "visibility": null,
    "device_id": null,
    "neura_id": "n7b0ashk4",
    "status": "active",
    "type": null,
    "vendor": null,
    "name": "Freddy",
    "lat": null,
    "lon": null,
    "mac": null,
    "ip": null,
    "created_at": 1430215590,
    "need_auth": false,
    "pending": false,
    "related_nodes": [ ],
    "image": "http://cdn.theneura.com/images/node/defaults/default_person.png",
    "labels": [ ],
    "_labels": [ ]
    }
}
```
# Instructions

Use postman (or any other tool which imitate API requests):

1. Under the **Normal** tab, select a POST request.
2. Under **Request URL** enter: wapi.theneura.com/api/nodes
3. For **Header** use the following params:
   3.1 **Content-Type**  application/json
   3.2 **Authorization** Bearer daac69bfdec1e980578588b26b5e2fb0749a82a117f50cbbdc922552ec66f855
4. In the raw tab insert:
    ```json
       {"node":{"name":"Freddy","node_type":"person", "contact_details":{
   "details" : {
       "first_name" : "Freddy",
       "last_name" : "Kruger",
       "phones" : [ 
          	 {
               	"phone" : "972501234567",
               	"type" : "mobile"
         	 	 }
     	  ]
  	 },
  	 "type" : "test"
	}
   }
}
### what you'll send: 
```
POST /api/nodes HTTP/1.1
Host: wapi.theneura.com
Content-Type: application/json
Authorization: Bearer daac69bfdec1e980578588b26b5e2fb0749a82a117f50cbbdc922552ec66f855
Cache-Control: no-cache
Postman-Token: f0cf3bfb-aa1a-43ac-4ab4-63f64c41a56e

{"node":{"name":"Freddy","node_type":"person", "contact_details":{
   "details" : {
       "first_name" : "Freddy",
       "last_name" : "Kruger",
       "phones" : [ 
          	 {
               	"phone" : "972501234567",
               	"type" : "mobile"
         	 	 }
     	  ]
  	 },
  	 "type" : "test"
	}
   }
}
```
