# cadastrobabi
```java
import java.time.LocalDateTime;

public class Main {
    public static void main(String[] args) {
        Evento feiraEmpregos = new Evento(
            "101",
            "Feira de Empregos 2025",
            "Centro de Convenções",
            CategoriaEvento.NETWORKING,
            LocalDateTime.now().plusDays(2).withHour(10).withMinute(0),
            480,
            "Conecte-se com empresas e explore novas oportunidades de carreira."
        );

        feiraEmpregos.adicionarParticipante("Empresa X");
        feiraEmpregos.adicionarParticipante("João Silva (Desenvolvedor)");
        feiraEmpregos.adicionarParticipante("Maria Souza (RH)");

        System.out.println(feiraEmpregos);
        System.out.println("Participantes confirmados: " + feiraEmpregos.getParticipantes());
    }
