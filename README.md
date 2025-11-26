# S_Architecture

### Como compilar?

Windows:
```
javac -cp "lib/junit-4.13.2.jar;src" -d bin src/architecture/*.java src/assembler/*.java src/components/*.java
```

Linux:
```
javac -cp "lib/junit-4.13.2.jar:src" -d bin src/architecture/*.java src/assembler/*.java src/components/*.java
```

O argumento "-d bin" envia todos os arquivos .class para o diretório bin. Só para organizar mesmo.

---

### Como rodar?

OBS: As extensões dos arquivos NÃO devem ser colocadas!

```
java -cp bin assembler.Assembler <arquivo.dsf>
```

O "arquivo.dsf" é lido pelo assembler e transformado em um executável "arquivo.dxf".

```
java -cp bin architecture.Architecture
```

O arquivo "program.dxf" e lido em modo de simulação, ou seja, instrução por instrução.

O argumento "-cp bin" serve para rodar um arquivo que não está na pasta atual. Os comandos assumem que você está na pasta raiz do programa.
