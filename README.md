# linux_driver_BCD_encode-decode
test for imx6ull
encode dts:gpio3.io2
          imx6_bcd{
              compatible = "fsl,imx6q-qiyang-bcd";
              bcd-gpios = <&gpio3 2 0>;
              status = "okay";
          };
decode dts:gpio3.io24
          imx6_bcd_decode{
              compatible = "fsl,imx6q-qiyang-bcd-decode";
              bcd-gpios = <&gpio3 24 0>;
              status = "okay";
              interrupt-parent = <&gpio3>;
              interrupts = <24 3>;
          };
