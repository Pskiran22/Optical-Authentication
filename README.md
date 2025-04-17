# OptAuth
**Novel Python image encryption: OpenCV processes a grayscale image, generating a secret key from random matrices. Encryption uses **FFT** and multiplication, showcasing complexity. Decryption reconstructs the original image, ensuring secure transmission and storage.**



In this image encryption and decryption process using Python, a novel approach is
employed to enhance the security of transmitted images. The algorithm leverages
the inherent characteristics of image matrices, introducing a secret key derived from
the element-wise multiplication of two random matrices. The method utilizes the
OpenCV library for image processing, employing a grayscale image loaded from a
file as the input.
The image's dimensions are extracted, providing insights into its structure with
height and width details. Subsequently, two random matrices are generated with the
same dimensions as the image, serving as the basis for the secret key. The secrecy of
the key lies in the unpredictability of the random matrices, adding an extra layer of
protection to the encryption process.
The encryption phase involves applying the Fast Fourier Transform (FFT) to the
input image, followed by element-wise multiplication with the secret key. The
resulting encrypted image is visually presented, showcasing the complexity
introduced by the encryption process, visible through a logarithmic transformation
of the absolute values.
To retrieve the original image, a decryption process is implemented. The encrypted
image undergoes division by the complex conjugate of the secret key, followed by an
inverse FFT to reconstruct the decrypted image. The final output demonstrates the
successful recovery of the original image, highlighting the effectiveness of the
encryption and decryption methodology.
This approach offers a unique perspective on image security, combining random
matrix generation and FFT techniques to safeguard sensitive visual information. The
visual representation of the encryption and decryption stages, along with the display
of the secret key, contributes to a comprehensive understanding of the proposed
image security technique. The encrypted image's complexity and the successful
reconstruction of the original image underscore the potential applications of this
method in secure image transmission and storage.

