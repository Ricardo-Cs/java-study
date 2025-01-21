# Maratona Java - Dev Dojo

[Canal Youtube DevDojo](https://youtube.com/playlist?list=PL62G310vn6nFIsOCC0H-C2infYgwm8SWW&si=R9KaZtRUnvXUU9Df)

---

### <a name="indice">Índice</a>

- [Aula 00: Introdução ao curso](#parte0)
- [Aula 01: O que esperar do curso](#parte1)
- [Aula 02: Como Java Funciona](#parte2)
- [Aula 03: Fazendo download da JDK 15](#parte3)
- [Aula 04: Configurando variáveis de ambiente](#parte4)
- [Aula 05: Executando compilação manualemente](#parte5)
- [Aula 06: Download da IDE Intellij Community](#parte6)
- [Aula 07: Conhecendo a IDE Intellij Community](#parte7)
- [Aula 08: Organizando o código em pacotes](#parte8)
- [Aula 09: Comentários](#parte9)
- [Aula 10: Tipos primitivos 1](#parte10)

---

## <a name="parte0">Aula 00: Introdução ao curso</a>

- https://youtu.be/VKjFuX91G5Q?si=yZqY7701oMWgHfJZ
- Aulas 00 - 09 são aulas introdutórias. Por isso não terão muitas anotações

[Voltar ao Índice](#indice)

---

## <a name="parte1">Aula 01: O que esperar do curso</a>

- https://youtu.be/ooCqalwSpuE?si=_ify9NpDDEgSy_1c

[Voltar ao Índice](#indice)

---

## <a name="parte2">Aula 02: Como Java Funciona</a>

- https://youtu.be/JasmdiTyduI?si=mDEjG1sOPEchte2k

[Voltar ao Índice](#indice)

---

## <a name="parte3">Aula 03: Fazendo download da JDK 15</a>

- https://youtu.be/Tsyeybeh968?si=Der8_oGrz8mv7L0b
- Baixei a JDK 21, uma versão mais recente.

[Voltar ao Índice](#indice)

---

## <a name="parte4">Aula 04: Configurando variáveis de ambiente</a>

- https://youtu.be/xzAESAp_soQ?si=JxpnN_bq4ri_n1jP

[Voltar ao Índice](#indice)

---

## <a name="parte5">Aula 05: Executando compilação manualmente</a>

- https://youtu.be/E64JTsEyXCM?si=itng_NbtHZSZtdEW
```java
public class HelloWorld {
    public static void main (String[] args) {
        System.out.println("Hello World!");
    } 
}
```
1. javac HelloWorld.java
2. java HelloWorld

[Voltar ao Índice](#indice)

---

## <a name="parte6">Aula 06: Download da IDE IntelliJ Community</a>

- https://youtu.be/uB5Qbm-RMyU?si=_FDR4XBmrhxhHWkz
- https://www.jetbrains.com/idea/download/?section=windows (Windows)

[Voltar ao Índice](#indice)

---

## <a name="parte7">Aula 07: Conhecendo a IDE IntelliJ Community</a>

- https://youtu.be/ds3t9C2A50U?si=6c7XqR3r5XhwKg5Q
- ctrl + f9 - Apenas build
- shift + f10 - Build e run do projeto
- ctrl + shift + f10 - Rebuild do projeto

[Voltar ao Índice](#indice)

---

## <a name="parte8">Aula 08: Organizando o código em pacotes</a>

- https://youtu.be/TnnS-R--WKc?si=sM9XvwuM8JDRndLb
- Nomes dos pacotes normalmente são a url do site inversa + nome do projeto + divisões, exemplo: br.com.devdojo.introducao
- Cada "ponto" será uma pasta, ou seja, a organização irá ficar: br/com/devdojo/introducao


[Voltar ao Índice](#indice)

---

## <a name="parte9">Aula 09: Comentários</a>

- https://youtu.be/2rMT0qRyiYs?si=m3y11umkY9H8GPOu
- Comentário de linha (//) - ctrl + /
- Comentários de linhas (/* ... */) - ctrl + shift + /
- JavaDoc (/** ... */) - alt + enter + "add javadoc"
- JavaDoc é utilizado para documentar classes, métodos ou atributos (mais recomendado entre as 3).

[Voltar ao Índice](#indice)

---

## <a name="parte10">Aula 10: Tipos primitivos 1 - Convenções de variáveis</a>

- https://youtu.be/RRHGYyJTTpQ?si=uw62veWMv0xz6kwR
- Tipos primitivos: int, double, float, char, byte, short, long, boolean
- Nomes de variáveis sempre começam com letras minúsculas e de preferência camelCase, exemplo: int idadeDaPessoa

[Voltar ao Índice](#indice)

---

## <a name="parte11">Aula 11: Tipos primitivos 2 - Declaração e tamanho em memória</a>

- https://youtu.be/veDgI_zZ7uk?si=jyxRebBFd4sn_-rg
    ```java
    public class Aula02TiposDeVariaveis {
        public static void main(String[] args) {
            // int, double, float, char, byte, short, long, boolean
            int idade = 10;
            long numeroGrande = 100000000;
            double salarioDouble = 2000;
            float salarioFloat = 2500;
            byte idadeByte = 10;
            short idadeShort = 10;
            boolean bool = true;
            char caractere = 'M';
            // Com exceção do boolean, todos são valores numéricos (char também suporta números).
            // A IDE identifica quando um valor atribuído ultrapassa o tamanho do tipo.
        }
    }
    ```

[Voltar ao Índice](#indice)

---

## <a name="parte12">Aula 12: Tipos primitivos 3 - Casting</a>

- https://youtu.be/74hd4o7V328?si=V1fbtBxPF8N2nkEt
- É possível especificar para o compilador que o valor atribuído a uma variável pertence ao mesmo tipo, por exemplo: 
    ```java
        double salarioDouble = 2000.0D;
        float salarioFloat = 2500.0F;
    ```
- Casting é como se você forçasse uma variável a receber um valor maior do que ele suporta, assim ele irá cortar bits para fazer caber o valor, dessa forma: 
    ```java
        int idade = (int) 10000000000L;
        float salarioFloat = (float) 2500.0D; // Nesse caso não cortará bits, pois cabe o valor. 
        long num = (long) 155.12; // Saída: 155  
    ```
- Casting não é recomendado.

[Voltar ao Índice](#indice)

---

## <a name="parte13">Aula 13: Tipos primitivos 4 - Strings</a>

- https://youtu.be/13VfcFXwsjw?si=yFee_cuPq2exlG-G
- Não é tipo primitivo, é uma classe, por isso é chamada com letra maiúscula.
    ```java
        String texto = "texto"; // Aspas duplas
        char caracter = 'A' // Aspas simples
    ```

[Voltar ao Índice](#indice)

---

## <a name="parte14">Aula 14: Tipos primitivos 5 - Exercício</a>

- https://youtu.be/Q0REhCVBvAg?si=l8u1WxDqvDKRz2ib

[Voltar ao Índice](#indice)

---