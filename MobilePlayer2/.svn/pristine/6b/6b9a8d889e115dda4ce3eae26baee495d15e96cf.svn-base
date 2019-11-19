package com.atguigu.mobileplayer2.view;

import android.content.Context;
import android.content.Intent;
import android.util.AttributeSet;
import android.view.View;
import android.widget.LinearLayout;
import android.widget.Toast;

import com.atguigu.mobileplayer2.R;
import com.atguigu.mobileplayer2.activity.SearchActivity;

/**
 * 作者：杨光福 on 2016/7/16 15:41
 * 微信：yangguangfu520
 * QQ号：541433511
 * 作用：自定义标题栏
 */
public class TitleBar extends LinearLayout implements View.OnClickListener {

    private View tv_search;

    private View rl_game;

    private View iv_record;
    private Context context;
    /**
     * 在代码中实例化该类的时候使用这个方法
     * @param context
     */
    public TitleBar(Context context) {
        this(context,null);
    }

    /**
     * 当在布局文件使用该类的时候，Android系统通过这个构造方法实例化该类
     * @param context
     * @param attrs
     */
    public TitleBar(Context context, AttributeSet attrs) {
        this(context, attrs,0);

    }

    /**
     * 当需要设置样式的时候，可以使用该方法
     * @param context
     * @param attrs
     * @param defStyleAttr
     */
    public TitleBar(Context context, AttributeSet attrs, int defStyleAttr) {
        super(context, attrs, defStyleAttr);
        this.context = context;
    }

    /**
     * 当布局文件加载完成的时候回调这个方法
     */
    @Override
    protected void onFinishInflate() {
        super.onFinishInflate();
        //得到孩子的实例
        tv_search = getChildAt(1);
        rl_game = getChildAt(2);
        iv_record = getChildAt(3);

        //设置点击事件
        tv_search.setOnClickListener(this);
        rl_game.setOnClickListener(this);
        iv_record.setOnClickListener(this);

    }

    @Override
    public void onClick(View v) {
        switch (v.getId()){
            case R.id.tv_search://搜索
//                Toast.makeText(context, "搜索", Toast.LENGTH_SHORT).show();
                Intent intent = new Intent(context,SearchActivity.class);
                context.startActivity(intent);
                break;
            case R.id.rl_game://游戏
                Toast.makeText(context, "游戏", Toast.LENGTH_SHORT).show();
                break;
            case R.id.iv_record://播放历史
                Toast.makeText(context, "播放历史", Toast.LENGTH_SHORT).show();
                break;
        }
    }
}
