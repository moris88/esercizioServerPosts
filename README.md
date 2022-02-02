# ServerPosts

Realizzare una interfaccia web (HTML & Javascript) che restituisca:
- 2 post,
- 5 commenti,
- 10 utenti,

da un servizio server gratuito chiamato [JsonPlaceholder](https://jsonplaceholder.typicode.com/).

Output che deve restituire:
    <code>
        <div>
            <p>POST:</p>
            <ul id='posts'>
                <li> post 1</li>
                <li> post 2</li>
                <li> ...</li>
                <li> post n</li>
            </ul>
        </div>
        <div>
            <p>COMMENTI:</p>
            <ul id='comments'>
                <li> comment 1</li>
                <li> comment 2</li>
                <li> ...</li>
                <li> comment n</li>
            </ul>
        </div>
        <div>
            <p>UTENTI:</p>
            <ul id='users'>
                <li> user 1</li>
                <li> user 2</li>
                <li> ...</li>
                <li> user n</li>
            </ul>
        </div>
    </code>


Consiglio:
- usare chiamate request http native di javascript [fetch](https://developer.mozilla.org/en-US/docs/Web/API/Fetch_API).

Esempio di request http:

    fetch('https://jsonplaceholder.typicode.com/todos/1')
        .then(response => response.json())
        .then(json => console.log(json))