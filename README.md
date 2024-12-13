# java-template

## 구현 기능 목록 템플리
    # 구현 기능 목록
        
    ## 기능 목록
        -[ ] xxx
        
    ## 입력 
        -[ ] xxx
        
    ## 출력
        -[ ] xxx
        
    ## 예외
        -[ ] xxx
## Controller
    private final InputView inputView;
    private final OutputView outputView;

    public Controller(InputView inputView, OutputView outputView) {
        this.inputView = inputView;
        this.outputView = outputView;
    }

    public void run() {
    }

## View
### InputView
    public class InputView {
        public String readLine() {
            String readLine = Console.readLine();
            return readLine.trim();
        }
    }

### OutputView
    public class OutputView {
        public void print(String message) {
            System.out.println(message);
        }
    }

## MESSAGE
    public class Message {
        Private static final String XXX = "";
    }
## ERROR MESSAGE
    public class ErrorMessage {
        Private static final String ERROR = "[ERROR]";
    }

## Parser
    public class Parser {
        public static int parseInt(String input) {
            try {
                return Integer.parseInt(input);
            }catch (Exception e) {
            throw new IllegalArgumentException(ErrorMessage.XXX);
            }
        }
    }      

## UNIT Comma
    public static final DecimalFormat NUMBER_FORMAT = new DecimalFormat("###,###");

    private String formatted(Integer value) {
        return NUMBER_FORMAT.format(value);
    }
