# pwmlib-opi
PWM Library for H3/H2+ Sunxi SoC

���̃��C�u������OrangePi��NanoPi�ȂǁAH3�x�[�X�̃}�V���Ńn�[�h�E�F�APWM���g�����߂̃��C�u�����ł��B  
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
period �S�̂̃p���X��  

void pwm_active(float period)  
period Active�̃p���X��  
