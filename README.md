!DOCTYPE html>
<html>
    <body>
        <script>
            function adiciona(){
                let inputNome= document.querySelector("#nome")
                let inputSobrenome = document.querySelector("#sobrenome")
                let inputIdade = document.querySelector("#idade")

                let tbody = document.querySelector("tbody");
                tbody.innerHTML +=`
                <tr>
                    <td>${inputNome.value}</td>
                    <td>${inputSobrenome.value}</td>
                    <td>${inputIdade.value}</td>
                </tr>
         `;
            }
        </script>
        <input type="text" id="nome" placeholder="Nome:" />
        <input type="text" id="sobrenome" placeholder="Sobrenome:" />
        <input type="text" id="idade" placeholder="Idade:" />
        <button onclick="adiciona()">Adicionar</button>
        <table>
            <thead>
                <tr>
                   <th>Nome</th>
                   <th>Sobrenome</th>
                   <th>Idade</th>
                </tr>
            </thead>
            <tbody>
                <tr>
                    <td>Joao Victor</td>
                    <td>Ferreira</td>
                    <td>19</td>
                </tr>
                <tr>
                    <td>Neymar</td>
                    <td>Jr</td>
                    <td>32</td>
                </tr>
            </tbody>
        </table>
    </body>
</html>
