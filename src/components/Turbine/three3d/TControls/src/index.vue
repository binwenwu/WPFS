<script>
import { OrbitControls } from "three/examples/jsm/controls/OrbitControls";
export default {
    name: "TControls",
    inject: ["global"],
    mounted() {
        /*esline-disable */
        const { camera, CSSRender } = this.global;
        let controls = new OrbitControls(camera, CSSRender.domElement);
        // controls.minDistance = 0.2;
        controls.maxDistance = 10.0;
        controls.maxPolarAngle = Math.PI * 0.9;
        this.global.controls = controls;
        this.global.controls.enablePan = true;
    },
    render(){
        return null 
    }
};
</script>
