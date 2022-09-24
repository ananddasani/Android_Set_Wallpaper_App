# Android_Set_Wallpaper_App
Setting Phon's Wallpaper From App only

This topic is a part of [My Complete Andorid Course](https://github.com/ananddasani/Android_Apps)

#### 1st Activity 
```
findViewById(R.id.button).setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {

                Bitmap bitmap = BitmapFactory.decodeResource(getResources(), R.drawable.my_snap);
                WallpaperManager wallpaperManager = WallpaperManager.getInstance(getApplicationContext());

                try {
                    wallpaperManager.setBitmap(bitmap);
                    Toast.makeText(MainActivity.this, "Wallpaper Changed :)", Toast.LENGTH_SHORT).show();
                } catch (IOException e) {
                    Toast.makeText(MainActivity.this, "Something went wong", Toast.LENGTH_SHORT).show();
                    e.printStackTrace();
                }
            }
        });
```

# App Highlight

<img src="app_images/Set Wallpater Code.png" width="1000" /><br>

<img src="app_images/Set Wallpaper App.png" width="300" /><br>
