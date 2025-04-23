<img src="https://octodex.github.com/images/welcometocat.png" align="right" height="250px" />

⭐️ Parabéns, gabrielaraujr! ⭐️

Você concluiu este exercício! Ótimo trabalho! 🥳

Se quiser praticar novamente, você pode repetir os passos abaixo. Basta clicar novamente no botão **Iniciar Exercício**.

> Dessa vez, a Mona não vai avaliar você! 😉

# API de Atividades da Escola Secundária Mergington

Uma aplicação extremamente simples usando FastAPI que permite aos estudantes visualizar e se inscrever em atividades extracurriculares.

## Funcionalidades

- Visualizar todas as atividades extracurriculares disponíveis
- Inscrever-se em atividades

## Como começar

1. Instale as dependências:

   ```
   pip install fastapi uvicorn
   ```

2. Execute a aplicação:

   ```
   python app.py
   ```

3. Abra seu navegador e acesse:
   - Documentação da API: http://localhost:8000/docs
   - Documentação alternativa: http://localhost:8000/redoc

## Endpoints da API

| Método | Endpoint                                                          | Descrição                                                                  |
| ------ | ----------------------------------------------------------------- | -------------------------------------------------------------------------- |
| GET    | `/activities`                                                     | Obter todas as atividades com detalhes e número atual de participantes     |
| POST   | `/activities/{activity_name}/signup?email=student@mergington.edu` | Inscrever-se em uma atividade                                              |

## Modelo de Dados

A aplicação utiliza um modelo de dados simples com identificadores claros:

1. **Atividades** - Usa o nome da atividade como identificador:

   - Descrição
   - Horários
   - Número máximo permitido de participantes
   - Lista de e-mails dos estudantes inscritos

2. **Estudantes** - Usa o e-mail como identificador:
   - Nome
   - Ano escolar

Todos os dados são armazenados em memória, portanto os dados serão redefinidos quando o servidor for reiniciado.
