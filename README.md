import { FunctionComponent, useCallback } from "react";
import { useNavigate } from "react-router-dom";
import "./SignIn.css";

const SignIn: FunctionComponent = () => {
  const navigate = useNavigate();

  const onRectangle2Click = useCallback(() => {
    navigate("/home-page");
  }, [navigate]);

  return (
    <div className="sign-in">
      <div className="frame">
        <div className="medsol">MedSoL</div>
        <img
          className="cdb3-76c1-473c-9370-136aab4633-icon"
          alt=""
          src="/2274cdb376c1473c9370136aab463338removebgpreview-1@2x.png"
        />
      </div>
      <div className="frame1">
        <div className="welcome">Welcome !</div>
        <div className="frame-child" />
        <div className="enter-your-username">Enter your username</div>
        <div className="frame-item" />
        <div className="enter-your-email">Enter your email</div>
        <div className="frame-inner" onClick={onRectangle2Click} />
        <div className="log-in">Log IN</div>
      </div>
    </div>
  );
};

export default SignIn;
