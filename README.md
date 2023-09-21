# lane_detection(opencv)

使用files.upload()從本地上傳一張圖像文件到Colab環境。

讀取上傳的圖像文件並顯示原始圖像。這裡使用OpenCV庫的cv2.imread()讀取圖像，然後使用plt.imshow()顯示圖像。

將原始圖像轉換為灰度圖像，這是為了後續的邊緣檢測。

對灰度圖像應用高斯平滑/模糊，以減少圖像中的噪聲。

調整Canny邊緣檢測的參數，並在模糊後的圖像上應用Canny邊緣檢測算法，以檢測圖像中的邊緣。

顯示Canny邊緣檢測結果圖像，其中檢測到的邊緣以白色顯示。

定義霍夫變換的相關參數，例如rho（距離分辨率）、theta（角度分辨率）、閾值等。

創建一個空白圖像，與原始圖像大小相同，用於在上面繪製檢測到的直線。

使用cv2.HoughLinesP()函數在Canny邊緣圖像上運行霍夫變換，以檢測直線。

在原始圖像上繪製檢測到的直線，並將它們以紅色顯示。

最後，將檢測到的直線圖像與原始圖像叠加，並顯示結果圖像，以突顯檢測到的直線。

程式碼的主要目的是在輸入圖像中檢測並顯示直線，它使用了圖像處理和計算機視覺技術來實現這一目標。
