# CS 347: Lab 14 – The People’s Dictionary

see: https://twodee.org/blog/18222

## Testing

1. `GET /words`

   - `curl -v localhost:5000/words`

1. `GET /:word`

   - `curl -v localhost:5000/duck`

1. `POST /:word`<ul><li>
   <pre>curl -v \
   --request POST \
   --header 'Content-Type: application/json' \
   --data '{"definition": "world wide web"}' \
   http://localhost:5000/www</pre>
   </li></ul>
1. `PATCH /:word/:definitionId/like`<ul><li>
     <pre>curl -v \
   --request PATCH \
   --header 'Content-Type: application/json' \
   --data '{"definition": "world wide web"}' \
   http://localhost:5000/www/8/like</pre>
     </li></ul>
1. `PATCH /:word/:definitionId`<ul><li>
     <pre>curl -v \
   --request PATCH \
   --header 'Content-Type: application/json' \
   --data '{"definition": "world wide webaroni!"}' \
   http://localhost:5000/www/8</pre>
     </li></ul>
1. `GET /search/:substring`
   - `curl -v localhost:5000/search/roni`
1. `DELETE /:word/:definitionId`<ul><li>
     <pre>curl -v \
   --request DELETE \
   http://localhost:5000/www/8</pre>
     </li></ul>
1. `DELETE /:word`<ul><li>
     <pre>curl -v \
   --request DELETE \
   http://localhost:5000/www</pre>
     </li></ul>
