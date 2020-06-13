# TextViewzuojia
TextView显示  修改文字

if(getId() == mContext.getResources().getIdentifier("item_hardware_text_desc","id","com.antutu.ABenchMark")
                && mContext.getClass().toString().contains("com.antutu.benchmark.ui.device.activity.ActivityDeviceInfo")){
                ViewParent viewParent = getParent();
                if(viewParent instanceof android.widget.LinearLayout) {
                View item_hardware_text_title = ((android.widget.LinearLayout)viewParent).getChildAt(0);
                        if(item_hardware_text_title instanceof TextView) {
                           if(((TextView)item_hardware_text_title).getText().toString().trim().equals("屏幕尺寸")){
                               String mstr=desPhysicalSize+" 英寸";
                                text=(CharSequence)mstr;
                           }
                           if(((TextView)item_hardware_text_title).getText().toString().trim().equals("Size")){
                               String mstr=desPhysicalSize+" inches";
                                text=(CharSequence)mstr;
                           }
                           if(((TextView)item_hardware_text_title).getText().toString().trim().equals("螢幕尺寸")){
                               String mstr=desPhysicalSize+" 英寸";
                                   text=(CharSequence)mstr;
                           }
                        }
                 }
               }
