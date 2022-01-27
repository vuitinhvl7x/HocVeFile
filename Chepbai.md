#ĐỌC GHI FILE
##THƯ VIỆN FILE
1. Có thể check xem đó có file không 
2. Có thể tạo/xóa ngay file trong code
3. Lấy đường dẫn tuyệt đối của file
![Screenshot](https://scontent.xx.fbcdn.net/v/t1.15752-9/p403x403/272326736_671311113881681_7511764882296480152_n.png?_nc_cat=100&ccb=1-5&_nc_sid=aee45a&_nc_ohc=af8oZmrjCiYAX8P6DZD&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AVJtiXlTVvsWRuiQCzfLtyQMuC1nFzxxTkzHQ8tXPvgW4w&oe=6216DE11)
##DataIn/Out - put
1.Dùng để nhập dữ liệu vào
![Screenshot](https://scontent.xx.fbcdn.net/v/t1.15752-9/272013603_350237950256918_5716590065533617490_n.png?_nc_cat=110&ccb=1-5&_nc_sid=aee45a&_nc_ohc=yrkLIeHlncUAX_qHRwZ&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AVKOThhZoQsVcBLP7xun9LbTkypgLTCbr-Pd4wBWGFLrEw&oe=621880BE)
##Thao tác với file bằng FileInputStream ( có thể xài cả 2 dạng binary/text)
![Screenshot](https://scontent-hel3-1.xx.fbcdn.net/v/t1.15752-9/272323289_1110207249738219_9119514370354027593_n.png?_nc_cat=103&ccb=1-5&_nc_sid=ae9488&_nc_ohc=hNVcVrZrtlgAX_YXsdx&_nc_ht=scontent-hel3-1.xx&oh=03_AVLKr1sStoqsY75iAXNvrxOkRbEhM9FwdkYz4MAAeMsCqw&oe=621632E8)
1. Luôn bắt try catch khi làm việc với file
2. Khai báo obj ngoài try - catch
3. Phải đóng file trong finally 
4. trong try
   1. biến ch chỉ để lấy mã của kí tự chứ không phải kí tự => cần covert về dạng char khi muốn xuất
   2. kí tự cuối cùng trong file luôn có giá trị = - 1
 
##Thao tác với file (text)
![Screeshot](https://scontent.xx.fbcdn.net/v/t1.15752-9/p403x403/272300435_741984470121784_4914142184224906658_n.png?_nc_cat=107&ccb=1-5&_nc_sid=aee45a&_nc_ohc=qcalAxk8jDUAX8Ax2Ys&_nc_oc=AQlNYW346MrLi2nvomH2gc048qvX0VpltJtW2SFj8or6-XhnKIEWWEEOUjMYyg0QIZkVolV2iNmJt2hKk1toAGmi&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AVI821V15sGsak-kpml2-UnCqOtI5kCMw4Unyh7KENc7Dg&oe=62181EE1)

1.Ngoài những lưu ý như thao tác trên: còn có thể viết tiếp vào cuối file 
##Thao tác với file bằng Buffered 
![Screeshot](https://scontent-hel3-1.xx.fbcdn.net/v/t1.15752-9/272048825_512303746833223_747657154387587778_n.png?_nc_cat=111&ccb=1-5&_nc_sid=ae9488&_nc_ohc=85JZzlNIp-IAX8u31eI&tn=Nh1sVwXKQts0v8tL&_nc_ht=scontent-hel3-1.xx&oh=03_AVKt_gj51_JQSJDHrl0WMDl3TjcZDu1TpIH3hDVYDP0J8Q&oe=6217FDC0)
##Lưu đối tượng vào file - ObjectStreamClass (Serialization - tuần tự hóa)
![Screenshot](https://scontent.xx.fbcdn.net/v/t1.15752-9/p403x403/272355989_4641921535926989_3544025467313146030_n.png?_nc_cat=103&ccb=1-5&_nc_sid=aee45a&_nc_ohc=dgLprxqcMc4AX-TxdxD&_nc_ad=z-m&_nc_cid=0&_nc_ht=scontent.xx&oh=03_AVKDo9YC8UwW-SjxijZZQmqvzuI1LFRes2Ilw2RAR_ca3g&oe=62166736)

Cần implements Serializable(  trong thư viện java.io )