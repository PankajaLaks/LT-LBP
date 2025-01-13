# LT-LBP

# Single Pixel Conversion

def get_pixel(img,center,x,y):
    n_value=0
    try:
        if img[x][y]>=center:
            n_value=1
    except:
        pass
    return n_value

 # LT-LBP Conversion with the neighbhoring pixels   

def LT=LBP(img,x,y):
    center=img[x][y]
    val_ar=[]      
    val_ar.append(get_pixel(img,center,x-1,y-1)) 
    val_ar.append(get_pixel(img,center,x-1,y))
    val_ar.append(get_pixel(img,center,x-1,y+1)) 
    val_ar.append(get_pixel(img,center,x,y+1))
    val_ar.append(get_pixel(img,center,x+1,y+1)) 
    val_ar.append(get_pixel(img,center,x+1,y)) 
    val_ar.append(get_pixel(img, center, x + 1, y-1))  
    val_ar.append(get_pixel(img, center, x, y-1))
    power_val = [0, 1, 2, 3, 4, 5, 6, 7]
    val = 0
    for i in range(len(val_ar)):
        val += val_ar[i] * power_val[i]     
    return val
