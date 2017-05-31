# Back End Challenge

Criar um projeto Django utilizando o TastyPie ou o Django REST framework como interface API REST.


## Documentaçes:

http://docs.djangoproject.com/en/ (>=1.9)

http://django-tastypie.readthedocs.io/en/

ou

http://www.django-rest-framework.org/tutorial/quickstart/


## Projeto:

* Criar uma aplicação simples com dois models (podendo ser Teacher e Student, Person e Pet, ou qualquer outra relação entre duas entidades)
* Criar um relacionamento one-to-many do model 1 para com o model 2
* Implementar todos os métodos de API: C/R/U/D 
   Obs: no GET, o model 2 deve retornar sua relação com o model 1 no resultado, como no exemplo abaixo:

```
{
    "objects": [
        {
            "name "Bobby",
            "id": "1",
            "resource_uri": "/api/v1/pet/1/",
            "person": {
                "name": "John",
                "resource_uri": "/api/v1/person/1/",
                "id": "1"
            }
        },
        {
            "name "Lilly",
            "id": "2",
            "resource_uri": "/api/v1/pet/2/",
            "person": {
                "name": "Robert",
                "resource_uri": "/api/v1/person/2/",
                "id": "2"
            }
        }
    ]
}
```
    

* Criar sistema de autenticação simples, por Basic Autentication (Header ou GET), para restringir o acesso aos dados.
* No DELETE do model 1, os registros do model 2 relacionados ao mesmo devem ser excluídos também.


## Publicação:

Publicar no GitHub ou enviar projeto compactado (zip) por email.
