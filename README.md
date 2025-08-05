📝 Lista de Tarefas com Java Collections
Este é um exercício guiado em Java para praticar o uso da classe ArrayList da API de Collections. O projeto foi desenvolvido acompanhando a professora Cami, durante o Bootcamp Santander 2025 da DIO, com foco em criar e manipular uma lista de tarefas.

📚 O que foi praticado:
Criar classes e objetos em Java;
Usar ArrayList da biblioteca java.util;
Adicionar e remover itens de uma lista;
Contar o total de elementos na lista;
Exibir todos os itens no console;
Usar toString() para facilitar a exibição no System.out.println().

🧱 Como funciona o projeto

📌 Classe Tarefa
Representa uma tarefa com um atributo descricao.


public class Tarefa {
    private String descricao;

    public Tarefa(String descricao) {
        this.descricao = descricao;
    }

    public String getDescricao() {
        return descricao;
    }

    @Override
    public String toString() {
        return descricao;
    }
}

📌 Classe ListaTarefa
Contém uma lista de objetos Tarefa e vários métodos para manipular essa lista.

Métodos:
adicionarTarefa(String descricao): Adiciona uma nova tarefa à lista.
removerTarefa(String descricao): Remove todas as tarefas com a descrição informada.
obterNumetoTotalTarefas(): Retorna a quantidade de tarefas.
obterDescricoesTarefas(): Mostra todas as tarefas.

▶️ Execução (main)
ListaTarefa listaTarefa = new ListaTarefa();

System.out.println("O número total de elementos na lista é: " + listaTarefa.obterNumetoTotalTarefas());

listaTarefa.adicionarTarefa("Tarefa 1");
listaTarefa.adicionarTarefa("Tarefa 1");
listaTarefa.adicionarTarefa("Tarefa 2");

System.out.println("O número total de elementos na lista é: " + listaTarefa.obterNumetoTotalTarefas());

listaTarefa.removerTarefa("Tarefa 1");

System.out.println("O número total de elementos na lista é: " + listaTarefa.obterNumetoTotalTarefas());

listaTarefa.obterDescricoesTarefas();

🖥️ Saída esperada:
O número total de elementos na lista é: 0
O número total de elementos na lista é: 3
O número total de elementos na lista é: 1
[Tarefa 2]
