Advanced Python Image Encryption Using OpenCV and FFT

This image encryption and decryption technique, developed in Python, presents an innovative method for securing grayscale images during transmission and storage. Utilizing the OpenCV library for image handling, the approach begins by importing a grayscale image from a file and determining its height and width to establish its matrix structure.

A core feature of the method is the creation of a secret key formed through the element-wise multiplication of two randomly generated matrices that share the same dimensions as the image. These random matrices introduce unpredictability, reinforcing the security of the encryption process.

The encryption stage employs the Fast Fourier Transform (FFT) to convert the image data into the frequency domain. The transformed image is then encrypted by multiplying it element-wise with the secret key. To visualize the result, a logarithmic scale is applied to the absolute values of the encrypted matrix, emphasizing the complexity and distortion added by the encryption.

Decryption reverses this process: the encrypted image is divided by the complex conjugate of the secret key, and then the Inverse FFT is applied to retrieve the original image. The successful restoration of the image verifies the robustness of the algorithm.

This technique stands out due to its use of random matrix-based key generation combined with FFT, offering a strong layer of protection against unauthorized access. The encrypted image's complexity, along with the clear restoration of the original, showcases the method's practicality in secure image communication systems. Visual outputs of both the encryption and decryption phases, along with the generated secret key, help illustrate the effectiveness of this approach in protecting sensitive image data.

