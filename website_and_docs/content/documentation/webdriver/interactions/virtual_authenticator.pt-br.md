---
title: "Virtual Authenticator"
linkTitle: "Virtual Authenticator"
weight: 16
description: >
    Uma representação do modelo Web Authenticator.
aliases: [
"/pt-br/documentation/webdriver/virtual_authenticator/"
]
---

Aplicações web podem habilitar um mecanismo de autenticação baseado em chaves públicas conhecido como Web Authentication para autenticar usuários sem usar uma senha. 
[Web Authentication](https://www.w3.org/TR/webauthn-2/) define APIs que permitem ao usuário criar uma credencial e registra-la com um autenticador. 
Um autenticador pode ser um dispositivo ou um software que guarde as chaves públicas do usuário e as acesse caso seja pedido. 

Como o nome sugere, Virtual Authenticator emula esses autenticadores para testes.

## Virtual Authenticator Options

Um Autenticador Virtual tem uma [série de propriedades](https://www.w3.org/TR/webauthn-2/#sctn-automation-virtual-authenticators).
Essas propriedades são mapeadas como VirtualAuthenticatorOptions nos bindings do Selenium.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L72-78" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L48-55" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< gh-codeblock path="examples/javascript/test/virtual_authenticator/virtualAuthenticatorOptions.spec.js#L10-L16" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}


## Add Virtual Authenticator

Cria um novo autenticador virtual com as propriedades fornecidas.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L85-92" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L63-71" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< gh-codeblock path="examples/javascript/test/virtual_authenticator/virtualAuthenticator.spec.js#L51-L55" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Remove Virtual Authenticator

Remove o autenticador virtual adicionado anteriormente.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L101-105" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#80-86" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< gh-codeblock path="examples/javascript/test/virtual_authenticator/virtualAuthenticator.spec.js#L62-L63" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Create Resident Credential

Cria uma resident (stateful) credential com os requeridos [parâmetros](https://w3c.github.io/webauthn/#sctn-automation-add-credential). 

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L120-123" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#103-107" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Create Non-Resident Credential 

Cria uma resident (stateless) credential com os requeridos [parâmetros](https://w3c.github.io/webauthn/#sctn-automation-add-credential). 

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L163-165" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L145-148" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Add Credential

Registra a credencial com o autenticador. 

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L157-166" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L139-150" >}}   
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Get Credential

Retorna a lista de credenciais que o autenticador possui.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L177-191" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L162-178" >}}  
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}


## Remove Credential

Remove a credencial do autenticador baseado na id da credencial passado.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L201-210" >}}
{{< /tab >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L189-198" >}} 
{{< tab header="CSharp" >}}
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}


## Remove All Credentials

Remove todas as credenciais do autenticador.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L216-225" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L207-216" >}} 
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}

## Set User Verified

Diz se o autenticador simulará sucesso ou falha na verificação de usuário.

{{< tabpane text=true langEqualsHeader=true >}}
{{< tab header="Java" >}}
{{< gh-codeblock path="examples/java/src/test/java/dev/selenium/virtual_authenticator/VirtualAuthenticatorTest.java#L231-232" >}}
{{< /tab >}}
{{< tab header="CSharp" >}}
{{< gh-codeblock path="examples/dotnet/SeleniumDocs/VirtualAuthentication/VirtualAuthenticatorTest.cs#L224-225" >}} 
{{< /tab >}}
{{< tab header="Ruby" >}}
{{< /tab >}}
{{< tab header="Python" >}}
{{< /tab >}}
{{< tab header="JavaScript" >}}
{{< /tab >}}
{{< tab header="Kotlin" >}}
{{< /tab >}}
{{< /tabpane >}}