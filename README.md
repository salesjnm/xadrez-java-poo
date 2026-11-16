# xadrez-java-poo
Atividade de um jogo de xadrez da disciplina de Programação Orientada à Objetos

## Perguntas para reflexão**

### 1. Por que a classe Peca é declarada como abstract?
Porque ela funciona apenas como um molde base para guardar as informações gerais que toda peça tem (nome, símbolo, cor e posição). 

### 2. O que acontece se você tentar fazer Peca p = new Peca(...) diretamente?
Dá erro de compilação (Peca *is abstract; cannot be instantiated*), porque o Java não permite instanciar diretamente uma classe abstrata.   

### 3. Por que movimentoValido() é abstrato em vez de ter uma implementação padrão?
Porque cada peça do xadrez anda de um jeito diferente, então não existe uma regra única que sirva para todas. Deixando o método abstrato, cada subclasse é obrigada a implementar a sua própria lógica de movimento.   

### 4. Qual a vantagem de usar Peca[][] no tabuleiro em vez de tipos específicos como Torre[][]?
Usando a matriz do tipo Peca[][], conseguimos armazenar qualquer tipo de peça na mesma estrutura graças à herança. S
