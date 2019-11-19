package com.atguigu.mobileplayer2.base;

import android.content.Context;
import android.view.View;

/**
 * 作者：杨光福 on 2016/7/16 11:36
 * 微信：yangguangfu520
 * QQ号：541433511
 * 作用：基类，公共类，
 * VideoPager
 * <p/>
 * AudioPager
 * <p/>
 * NetVideoPager
 * <p/>
 * NetAudioPager
 * 都继承该类
 */
public abstract class BasePager {

    /**
     * 上下文
     */
    public final Context context;
    /**
     * 接收各个页面的实例
     */
    public View rootView;
    public boolean isInitData;

    public BasePager(Context context) {
        this.context = context;
        rootView = initView();
    }

    /**
     * 强制子页面实现该方法，实现想要的特定的效果
     *
     * @return
     */
    public abstract View initView();


    /**
     * 当子页面，需要绑定数据，或者联网请求数据并且绑定的时候，重写该方法
     */
    public void initData(){

    }
}
