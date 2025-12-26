import java.time.LocalDateTime;
import java.time.format.DateTimeFormatter;
import java.util.Base64;

// Спільний інтерфейс для повідомлень
interface Message {
    String getContent();
}

// Базовий клас повідомлення
class SimpleMessage implements Message {
    private String text;

public SimpleMessage(String text) {
        this.text = text;
    }

@Override
    public String getContent() {
        return text;
    }
}                                                                                                
