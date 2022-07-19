# Underwater image enhancement
 
Generater model : structure of generator model is taken from UWGAN 
 
![alt text](https://github.com/sachin327/Underwater-image-enhancement/blob/main/Screenshot%20(219)%20-%20Copy.png)

here we used skip connections and msdb layers to improve performance of our model.

# MSDB LAYERS
 
![alt text](https://github.com/sachin327/Underwater-image-enhancement/blob/main/Screenshot%20(220).png)
![alt text](https://github.com/sachin327/Underwater-image-enhancement/blob/main/Screenshot%20(221).png)
![alt text](https://github.com/sachin327/Underwater-image-enhancement/blob/main/Screenshot%20(222).png)
 
Discriminator model : For discriminator model I have used the inception model cause it is very good at discriminating images even they are almost same.
 

Loss function :
 
loss = Lgan (D, G) + λ1 * L1(G)
 
Lgan  = Ex *[log D(x)] + Ey*[log(1 − D(G(y)))] 
 
L1 is abslute distance between the original image and the generated image.
 
λ1 is set to 50
