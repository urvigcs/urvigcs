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
.medsol {
  position: absolute;
  top: 5px;
  left: 126px;
  display: inline-block;
  width: 184px;
  height: 44px;
}
.cdb3-76c1-473c-9370-136aab4633-icon {
  position: absolute;
  top: 0;
  left: 0;
  width: 86.1px;
  height: 100px;
  object-fit: cover;
}
.frame,
.welcome {
  position: absolute;
}
.frame {
  top: 49px;
  left: 36px;
  width: 310px;
  height: 100px;
  overflow: hidden;
}
.welcome {
  top: 28px;
  left: 106px;
  color: var(--color-gray-300);
  display: inline-block;
  width: 175px;
  height: 42px;
}
.frame-child {
  position: absolute;
  top: 143px;
  left: 46px;
  border-radius: var(--br-3xs);
  background-color: var(--color-gainsboro);
  width: 299px;
  height: 67px;
}
.enter-your-username {
  position: absolute;
  top: 159px;
  left: 105px;
  font-size: var(--font-size-xl);
  display: inline-block;
  width: 175px;
  height: 42px;
}
.frame-item {
  position: absolute;
  top: 267px;
  left: 46px;
  border-radius: var(--br-3xs);
  background-color: var(--color-gainsboro);
  width: 299px;
  height: 67px;
}
.enter-your-email {
  position: absolute;
  top: 284px;
  left: 99px;
  font-size: var(--font-size-xl);
  display: inline-block;
  width: 175px;
  height: 42px;
}
.frame-inner {
  position: absolute;
  top: 422px;
  left: 20px;
  border-radius: var(--br-3xs);
  background-color: var(--color-thistle);
  width: 351px;
  height: 98px;
  cursor: pointer;
}
.log-in {
  position: absolute;
  top: 446px;
  left: 102px;
  display: inline-block;
  width: 175px;
  height: 42px;
}
.frame1,
.sign-in {
  height: 844px;
  overflow: hidden;
}
.frame1 {
  position: absolute;
  top: 182px;
  left: 0;
  border-radius: 60px;
  background-color: #a4a1cc;
  width: 390px;
  text-align: center;
  font-size: var(--font-size-17xl);
  color: var(--color-gray-400);
}
.sign-in {
  position: relative;
  border-radius: var(--br-21xl);
  background: linear-gradient(rgba(43, 93, 222, 0.2), rgba(43, 93, 222, 0.2)),
    #fff;
  width: 100%;
  text-align: left;
  font-size: var(--font-size-41xl);
  color: var(--color-gray-200);
  font-family: var(--font-jockey-one);
}



export default SignIn;
