package com.example.tryeventbus_simple;

import android.app.Activity;
import android.os.Bundle;
import android.view.View;
import android.widget.Button;

import com.harvic.other.FirstEvent2;

import de.greenrobot.event.EventBus;

public class SecondActivity extends Activity {
	private Button btn_FirstEvent;

	@Override
	protected void onCreate(Bundle savedInstanceState) {
		super.onCreate(savedInstanceState);
		setContentView(R.layout.activity_second);
		btn_FirstEvent = (Button) findViewById(R.id.btn_first_event);

		btn_FirstEvent.setOnClickListener(new View.OnClickListener() {

			@Override
			public void onClick(View v) {
				// TODO Auto-generated method stub
				//4.发消息
				EventBus.getDefault().post(new FirstEvent2("FirstEvent2 btn clicked aaaaaaaaaaaaaaa"));
			}
		});


	}

}
