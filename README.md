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

�T�[�{���[�^���g���ꍇ�A�S�̂̃p���X����Active�p���X���Ő��䂷�邱�Ƃ��ł��܂��B  
void pwm_begin(float period)  
period : �S�̂̃p���X��(mSec)  

void pwm_active(float period)  
period : Active�̃p���X��(mSec)  

---

![sg90-1](https://cloud.githubusercontent.com/assets/6020549/24579311/a6b02e34-172d-11e7-82ad-8dacc48f609b.JPG)

---

This is the library to use hardware PWM by a board of H3/H2+ base such as OrangePi and NanoPi.  
It works by the following board.  
OrangePi PC(H3)  
OrangePi ZERO(H2+)  
NanoPi M1(H3)

You have to make the following driver effective to use this library.  
https://github.com/iboguslavsky/pwm-sunxi-opi0  

---

SG90 micro servomotor (http://akizukidenshi.com/download/ds/towerpro/SG90.pdf) works by the following program.  

cc -o pwm pwm.c -lwiringPi  
sudo ./pwm  

When using a servomotor, you can control with entire pulse width and active pulse width.  

void pwm_begin(float period)  
period : entire pulse width(mSec)  

void pwm_active(float period)  
period :  active pulse width(mSec)  

