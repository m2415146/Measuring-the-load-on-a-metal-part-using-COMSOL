# Measuring-the-load-on-a-metal-part-using-COMSOL
a training task performed in a computer simulation class using COMSOL multiphysics

## Materials and methods

COMSOL multiphysics 6.2

Scheme and sizes

![5426890405305249700](https://github.com/user-attachments/assets/e4786805-a4ae-410a-a49a-e5971cefa92e)

MAterial ASTM A289, parameters: 

![Screenshot_261](https://github.com/user-attachments/assets/5279c798-748f-4897-a2fc-eb1dc408a224)

Load:

![Screenshot_262](https://github.com/user-attachments/assets/778a46f4-644d-4f26-a0b8-9118a15d501d)

## Create model

Model wizard/ 3d / SOlid mechanics / Stationary

Geometry/ mm

Geometry/ cylinder 

in the values from the diagram, we take into account that the diameters are indicated there, and the program allows you to enter the radius, so divide by 2

![Screenshot_263](https://github.com/user-attachments/assets/2536e365-d746-480e-b2dd-9c9be818d061)

Geometry/ booleans and partitions / difference

![Screenshot_265](https://github.com/user-attachments/assets/a5586670-f232-4aca-831e-6af87583859e)

result

![Screenshot_266](https://github.com/user-attachments/assets/547ffa71-7677-47ff-8d37-88ea8c2e936c)

materials: ASTM A289 [forging, radial,tested at 20 °C (293 K), R = -1, axial, total strain amplitude]

here we record the properties of the material given to us in the task

![Screenshot_267](https://github.com/user-attachments/assets/7212d36f-8485-4672-95ba-9269154f665a)

Fixed constrait - lowe radial part

![Screenshot_268](https://github.com/user-attachments/assets/3a81d0a1-0bc1-4782-a359-070e75e2e457)

Boundary load - use from task (pay attention to the load vector - we indicate it with a minus sign on the X-axis so that it acts in the direction we need)

![Screenshot_269](https://github.com/user-attachments/assets/af122544-b36b-4589-9a18-4f3e4b9a56ed)

Do not forget to mesh a model

![Screenshot_270](https://github.com/user-attachments/assets/7e8ddacd-cba2-491c-b422-fabf21370c96)

It's not necessary to use Extremely Fine quality, but I decided that my computer could handle it, even though it took longer than I had planned.

Study/ compute

Result

![Screenshot_271](https://github.com/user-attachments/assets/547e6989-a51f-4bc9-9175-4017f29b2d84)

## analysis of the results

the greatest stresses (red zone) are concentrated at the transition point from the cylindrical rod to the flange, on the inner surface of the flange, around the hole in the rod. There is also a small stress concentration at the junction of the rod with the flange. The screenshot shows the von Mises stress. This is an equivalent stress that is used to evaluate the flowability and strength of a material under a complex stress state (when several stresses are acting simultaneously). The maximum voltage is approximately 6 x 10^4 N/m2 = 60 MPa (megapascals).










