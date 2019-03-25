# ShowTime
Button In Grid Layout


### Priview
![ezgif com-resize (1)](https://user-images.githubusercontent.com/43386555/54909207-3d70ec00-4f1c-11e9-81b3-1b79c68db94c.gif)

### Source
    public class MainActivity extends AppCompatActivity {

        TextView textView;
        Button button1, button2, button3, button4, button5, button6, button7, button8, button9, button10, resetButton;

        @Override
        protected void onCreate(Bundle savedInstanceState) {
            super.onCreate(savedInstanceState);
            setContentView(R.layout.activity_main);

            textView = (TextView) findViewById(R.id.textView);
            button9 = (Button) findViewById(R.id.button9);
            button8 = (Button) findViewById(R.id.button8);
            button7 = (Button) findViewById(R.id.button7);
            button4 = (Button) findViewById(R.id.button4);
            button5 = (Button) findViewById(R.id.button5);
            button6 = (Button) findViewById(R.id.button6);
            button1 = (Button) findViewById(R.id.button1);
            button2 = (Button) findViewById(R.id.button2);
            button3 = (Button) findViewById(R.id.button3);
            button10 = (Button) findViewById(R.id.button10);
            resetButton = (Button) findViewById(R.id.resetButton);
        }

        public void putNumbertoView(String num) {

            textView.setText(num + "");

        }

        public void onQuestion(View view) {
            switch (view.getId()) {

                case R.id.button9:
                    putNumbertoView("9");
                    break;

                case R.id.button8:
                    putNumbertoView("8");
                    break;

                case R.id.button7:
                    putNumbertoView("7");
                    break;

                case R.id.button4:
                    putNumbertoView("4");
                    break;

                case R.id.button5:
                    putNumbertoView("5");
                    break;

                case R.id.button6:
                    putNumbertoView("6");
                    break;

                case R.id.button1:
                    putNumbertoView("1");
                    break;

                case R.id.button2:
                    putNumbertoView("2");
                    break;

                case R.id.button3:
                    putNumbertoView("3");
                    break;

                case R.id.button10:
                    putNumbertoView("10");
                    break;

                case R.id.resetButton:
                    putNumbertoView("");
                    break;
            }

        }
    }
