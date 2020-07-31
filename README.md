    @Override
    protected void onResume() {
        super.onResume();
        Intent intent = getIntent();
        String message = intent.getStringExtra(MainActivity.EXTRA_MESSAGE);
        TextView textView = findViewById(R.id.textView);
        if (android.os.Build.VERSION.SDK_INT >= android.os.Build.VERSION_CODES.O) {
            OffsetTime offset = OffsetTime.now();
            if (offset.getHour()>=6 && offset.getHour()<12){
                textView.setText("Good Morning "+ message);
            }
            else if (offset.getHour()>=12 && offset.getHour()<17){
                textView.setText("Good Afternoon "+ message);

            }
            else if (offset.getHour()>=17 && offset.getHour()<20){
                textView.setText("Good Evening "+ message);
            }

            else if (offset.getHour()>=20 || offset.getHour()<6){
                textView.setText("Good Night "+ message);
            }
        }
    }
