# petstore-api
This spec is mainly for testing Petstore server and contains fake endpoints, models. Please do not use this for any other purpose. Special characters: \" \\

This Python package is automatically generated by the [OpenAPI Generator](https://openapi-generator.tech) project:

- API version: 1.0.0
- Package version: 1.0.0
- Build package: org.openapitools.codegen.languages.PythonClientCodegen

## Requirements.

Python 2.7 and 3.4+

## Installation & Usage
### pip install

If the python package is hosted on a repository, you can install directly using:

```sh
pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git
```
(you may need to run `pip` with root permission: `sudo pip install git+https://github.com/GIT_USER_ID/GIT_REPO_ID.git`)

Then import the package:
```python
import petstore_api
```

### Setuptools

Install via [Setuptools](http://pypi.python.org/pypi/setuptools).

```sh
python setup.py install --user
```
(or `sudo python setup.py install` to install the package for all users)

Then import the package:
```python
import petstore_api
```

## Getting Started

Please follow the [installation procedure](#installation--usage) and then run the following:

```python
from __future__ import print_function
import time
import petstore_api
from petstore_api.rest import ApiException
from pprint import pprint


# Defining host is optional and default to http://petstore.swagger.io:80/v2
configuration.host = "http://petstore.swagger.io:80/v2"
# Create an instance of the API class
api_instance = petstore_api.AnotherFakeApi(petstore_api.ApiClient(configuration))
body = petstore_api.Client() # Client | client model

try:
    # To test special tags
    api_response = api_instance.call_123_test_special_tags(body)
    pprint(api_response)
except ApiException as e:
    print("Exception when calling AnotherFakeApi->call_123_test_special_tags: %s\n" % e)

```

## Documentation for API Endpoints

All URIs are relative to *http://petstore.swagger.io:80/v2*

Class | Method | HTTP request | Description
------------ | ------------- | ------------- | -------------
*AnotherFakeApi* | [**call_123_test_special_tags**](docs/AnotherFakeApi.md#call_123_test_special_tags) | **PATCH** /another-fake/dummy | To test special tags
*FakeApi* | [**create_xml_item**](docs/FakeApi.md#create_xml_item) | **POST** /fake/create_xml_item | creates an XmlItem
*FakeApi* | [**fake_outer_boolean_serialize**](docs/FakeApi.md#fake_outer_boolean_serialize) | **POST** /fake/outer/boolean | 
*FakeApi* | [**fake_outer_composite_serialize**](docs/FakeApi.md#fake_outer_composite_serialize) | **POST** /fake/outer/composite | 
*FakeApi* | [**fake_outer_number_serialize**](docs/FakeApi.md#fake_outer_number_serialize) | **POST** /fake/outer/number | 
*FakeApi* | [**fake_outer_string_serialize**](docs/FakeApi.md#fake_outer_string_serialize) | **POST** /fake/outer/string | 
*FakeApi* | [**test_body_with_file_schema**](docs/FakeApi.md#test_body_with_file_schema) | **PUT** /fake/body-with-file-schema | 
*FakeApi* | [**test_body_with_query_params**](docs/FakeApi.md#test_body_with_query_params) | **PUT** /fake/body-with-query-params | 
*FakeApi* | [**test_client_model**](docs/FakeApi.md#test_client_model) | **PATCH** /fake | To test \&quot;client\&quot; model
*FakeApi* | [**test_endpoint_parameters**](docs/FakeApi.md#test_endpoint_parameters) | **POST** /fake | Fake endpoint for testing various parameters  假端點  偽のエンドポイント  가짜 엔드 포인트
*FakeApi* | [**test_enum_parameters**](docs/FakeApi.md#test_enum_parameters) | **GET** /fake | To test enum parameters
*FakeApi* | [**test_group_parameters**](docs/FakeApi.md#test_group_parameters) | **DELETE** /fake | Fake endpoint to test group parameters (optional)
*FakeApi* | [**test_inline_additional_properties**](docs/FakeApi.md#test_inline_additional_properties) | **POST** /fake/inline-additionalProperties | test inline additionalProperties
*FakeApi* | [**test_json_form_data**](docs/FakeApi.md#test_json_form_data) | **GET** /fake/jsonFormData | test json serialization of form data
*FakeApi* | [**test_query_parameter_collection_format**](docs/FakeApi.md#test_query_parameter_collection_format) | **PUT** /fake/test-query-paramters | 
*FakeClassnameTags123Api* | [**test_classname**](docs/FakeClassnameTags123Api.md#test_classname) | **PATCH** /fake_classname_test | To test class name in snake case
*PetApi* | [**add_pet**](docs/PetApi.md#add_pet) | **POST** /pet | Add a new pet to the store
*PetApi* | [**delete_pet**](docs/PetApi.md#delete_pet) | **DELETE** /pet/{petId} | Deletes a pet
*PetApi* | [**find_pets_by_status**](docs/PetApi.md#find_pets_by_status) | **GET** /pet/findByStatus | Finds Pets by status
*PetApi* | [**find_pets_by_tags**](docs/PetApi.md#find_pets_by_tags) | **GET** /pet/findByTags | Finds Pets by tags
*PetApi* | [**get_pet_by_id**](docs/PetApi.md#get_pet_by_id) | **GET** /pet/{petId} | Find pet by ID
*PetApi* | [**update_pet**](docs/PetApi.md#update_pet) | **PUT** /pet | Update an existing pet
*PetApi* | [**update_pet_with_form**](docs/PetApi.md#update_pet_with_form) | **POST** /pet/{petId} | Updates a pet in the store with form data
*PetApi* | [**upload_file**](docs/PetApi.md#upload_file) | **POST** /pet/{petId}/uploadImage | uploads an image
*PetApi* | [**upload_file_with_required_file**](docs/PetApi.md#upload_file_with_required_file) | **POST** /fake/{petId}/uploadImageWithRequiredFile | uploads an image (required)
*StoreApi* | [**delete_order**](docs/StoreApi.md#delete_order) | **DELETE** /store/order/{order_id} | Delete purchase order by ID
*StoreApi* | [**get_inventory**](docs/StoreApi.md#get_inventory) | **GET** /store/inventory | Returns pet inventories by status
*StoreApi* | [**get_order_by_id**](docs/StoreApi.md#get_order_by_id) | **GET** /store/order/{order_id} | Find purchase order by ID
*StoreApi* | [**place_order**](docs/StoreApi.md#place_order) | **POST** /store/order | Place an order for a pet
*UserApi* | [**create_user**](docs/UserApi.md#create_user) | **POST** /user | Create user
*UserApi* | [**create_users_with_array_input**](docs/UserApi.md#create_users_with_array_input) | **POST** /user/createWithArray | Creates list of users with given input array
*UserApi* | [**create_users_with_list_input**](docs/UserApi.md#create_users_with_list_input) | **POST** /user/createWithList | Creates list of users with given input array
*UserApi* | [**delete_user**](docs/UserApi.md#delete_user) | **DELETE** /user/{username} | Delete user
*UserApi* | [**get_user_by_name**](docs/UserApi.md#get_user_by_name) | **GET** /user/{username} | Get user by user name
*UserApi* | [**login_user**](docs/UserApi.md#login_user) | **GET** /user/login | Logs user into the system
*UserApi* | [**logout_user**](docs/UserApi.md#logout_user) | **GET** /user/logout | Logs out current logged in user session
*UserApi* | [**update_user**](docs/UserApi.md#update_user) | **PUT** /user/{username} | Updated user


## Documentation For Models

 - [AdditionalPropertiesAnyType](docs/AdditionalPropertiesAnyType.md)
 - [AdditionalPropertiesArray](docs/AdditionalPropertiesArray.md)
 - [AdditionalPropertiesBoolean](docs/AdditionalPropertiesBoolean.md)
 - [AdditionalPropertiesClass](docs/AdditionalPropertiesClass.md)
 - [AdditionalPropertiesInteger](docs/AdditionalPropertiesInteger.md)
 - [AdditionalPropertiesNumber](docs/AdditionalPropertiesNumber.md)
 - [AdditionalPropertiesObject](docs/AdditionalPropertiesObject.md)
 - [AdditionalPropertiesString](docs/AdditionalPropertiesString.md)
 - [Animal](docs/Animal.md)
 - [ApiResponse](docs/ApiResponse.md)
 - [ArrayOfArrayOfNumberOnly](docs/ArrayOfArrayOfNumberOnly.md)
 - [ArrayOfNumberOnly](docs/ArrayOfNumberOnly.md)
 - [ArrayTest](docs/ArrayTest.md)
 - [BigCat](docs/BigCat.md)
 - [BigCatAllOf](docs/BigCatAllOf.md)
 - [Capitalization](docs/Capitalization.md)
 - [Cat](docs/Cat.md)
 - [CatAllOf](docs/CatAllOf.md)
 - [Category](docs/Category.md)
 - [ClassModel](docs/ClassModel.md)
 - [Client](docs/Client.md)
 - [Dog](docs/Dog.md)
 - [DogAllOf](docs/DogAllOf.md)
 - [EnumArrays](docs/EnumArrays.md)
 - [EnumClass](docs/EnumClass.md)
 - [EnumTest](docs/EnumTest.md)
 - [File](docs/File.md)
 - [FileSchemaTestClass](docs/FileSchemaTestClass.md)
 - [FormatTest](docs/FormatTest.md)
 - [HasOnlyReadOnly](docs/HasOnlyReadOnly.md)
 - [List](docs/List.md)
 - [MapTest](docs/MapTest.md)
 - [MixedPropertiesAndAdditionalPropertiesClass](docs/MixedPropertiesAndAdditionalPropertiesClass.md)
 - [Model200Response](docs/Model200Response.md)
 - [ModelReturn](docs/ModelReturn.md)
 - [Name](docs/Name.md)
 - [NumberOnly](docs/NumberOnly.md)
 - [Order](docs/Order.md)
 - [OuterComposite](docs/OuterComposite.md)
 - [OuterEnum](docs/OuterEnum.md)
 - [Pet](docs/Pet.md)
 - [ReadOnlyFirst](docs/ReadOnlyFirst.md)
 - [SpecialModelName](docs/SpecialModelName.md)
 - [Tag](docs/Tag.md)
 - [TypeHolderDefault](docs/TypeHolderDefault.md)
 - [TypeHolderExample](docs/TypeHolderExample.md)
 - [User](docs/User.md)
 - [XmlItem](docs/XmlItem.md)


## Documentation For Authorization


## api_key

- **Type**: API key
- **API key parameter name**: api_key
- **Location**: HTTP header


## api_key_query

- **Type**: API key
- **API key parameter name**: api_key_query
- **Location**: URL query string


## http_basic_test

- **Type**: HTTP basic authentication


## petstore_auth

- **Type**: OAuth
- **Flow**: implicit
- **Authorization URL**: http://petstore.swagger.io/api/oauth/dialog
- **Scopes**: 
 - **write:pets**: modify pets in your account
 - **read:pets**: read your pets


## Author



