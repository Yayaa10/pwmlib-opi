# pwmlib-opi
PWM Library for H3/H2+ Sunxi SoC

���̃��C�u������OrangePi��NanoPi�ȂǁAH3/H2+�x�[�X�̃{�[�h�Ńn�[�h�E�F�APWM���g�����߂̃��C�u�����ł��B  
�ȉ��̃{�[�h�œ�����m�F���Ă��܂��B  
OrangePi PC(H3)  
OrangePi ZERO(H2+)  
NanoPi M1(H3)

���̃��C�u�������g�����߂ɂ͈ȉ��̃h���C�o�[��L���ɂ���K�v���L��܂��B  
https://github.com/iboguslavsky/pwm-sunxi-opi0  

---

�ȉ��̃v���O������SG90�}�C�N���T�[�{���[�^�� 0���� -90�� �� +90�� �� 0�� �ɓ����܂��B  
cc -o pwm pwm.c -lwiringPi  
sudo ./pwm  

void pwm_begin(float period)  
period : �S�̂̃p���X��  

void pwm_active(float period)  
period : Active�̃p���X��  

---

This library is the library to use hardware PWM by a board of H3/H2+ base such as OrangePi and NanoPi.  
I'm confirming that it works by the following board.  
OrangePi PC(H3)  
OrangePi ZERO(H2+)  
NanoPi M1(H3)

You have to make the following driver effective to use this library.  
https://github.com/iboguslavsky/pwm-sunxi-opi0  

---

SG90 micro servomotor works by the following program.  
cc -o pwm pwm.c -lwiringPi  
sudo ./pwm  

void pwm_begin(float period)  
period : entire pulse width(mSec)  

void pwm_active(float period)  
period :  active pulse width(mSec)  

